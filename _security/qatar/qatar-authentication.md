---
api_key_in: []
api_specs:
- filename: qatar-qu-sso-oidc-openapi.yml
  format: yaml
  label: Qatar University Single Sign-On (OpenID Connect / OAuth 2.0)
  slug: qu-sso-oidc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qatar/refs/heads/main/openapi/qatar-qu-sso-oidc-openapi.yml
- filename: qatar-qupress-oai-pmh-openapi.yml
  format: yaml
  label: QU Press Open Journal System OAI-PMH API
  slug: qupress-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qatar/refs/heads/main/openapi/qatar-qupress-oai-pmh-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- saml
description: Qatar University's public programmable surfaces divide cleanly. Everything that harvests or reads scholarly metadata is open and anonymous — the QU Press OJS OAI-PMH endpoint that the university operates itself, and the QSpace repository endpoints that its hosting provider operates for it. Everything that touches a person is behind the university's own OpenID Connect / SAML provider at sso.qu.edu.qa, and there is no public onboarding path to it. No Qatar University surface issues API keys to the public, and none was found that documents an authentication model in prose.
kind: authentication
layout: security
method: probed
name: Qatar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qatar University secures its APIs with none, oauth2, openIdConnect, and saml across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Qatar University
provider_slug: qatar
scheme_count: 7
schemes:
- applies_to: https://qspace.qu.edu.qa/server/oai/request
  description: OAI-PMH harvesting is fully anonymous. Identify, ListMetadataFormats, ListSets, ListIdentifiers, ListRecords and GetRecord all answer 200 with no credential and no rate-limit header. The repository publishes no harvesting policy.
  evidence:
    status: 200
    url: https://qspace.qu.edu.qa/server/oai/request?verb=Identify
  name: QSpaceOaiPublic
  operator: tenant
  operator_basis: qspace.qu.edu.qa CNAMEs to qataru.cname.openrepository.com and resolves to 3.255.61.143 (Amazon eu-west-1). Open Repository is a commercial hosted-DSpace service; the hostname, content and Handle prefix are Qatar University's, the deployment is not.
  type: none
- applies_to: https://qspace.qu.edu.qa/server/api
  description: DSpace 7.6 read operations — the service root, communities, collections, items and discovery search — are anonymous. Write operations require a DSpace account and a CSRF token (DSpace's `DSPACE-XSRF-TOKEN` header exchange); no public registration path was found, so the write half of the API is not reachable by the public.
  evidence:
    status: 200
    url: https://qspace.qu.edu.qa/server/api
  name: QSpaceRestPublicRead
  operator: tenant
  type: none
- applies_to: https://qspace.qu.edu.qa/server/opensearch
  description: OpenSearch description and Atom/RSS result feeds are anonymous.
  evidence:
    status: 200
    url: https://qspace.qu.edu.qa/server/opensearch/service
  name: QSpaceOpenSearchPublic
  operator: tenant
  type: none
- applies_to: https://journals.qu.edu.qa/index.php/index/oai
  description: QU Press OJS OAI-PMH harvesting is anonymous over all nine journals. The adjacent OJS REST API at /index.php/{journal}/api/v1/ is NOT public — it returns 403 to unauthenticated callers, and OJS gates it behind an API token issued per user account.
  evidence:
    status: 200
    url: https://journals.qu.edu.qa/index.php/index/oai?verb=Identify
  name: QuPressOaiPublic
  operator: institution
  type: none
- applies_to: https://sso.qu.edu.qa
  caveats:
  - The discovery document is at a non-standard location. RFC 8414 says to append /.well-known/openid-configuration to the issuer; here it is nested under /oauth2/token/, and the issuer itself (https://sso.qu.edu.qa:9443/oauth2endpoints/token) points at the WSO2 management port. A conformant client discovering by the book will not find it.
  - The host serves an incomplete TLS chain, so a default OpenSSL-based client cannot read the discovery document at all. See identity-federation/qatar-identity-federation.yml.
  - /oauth2/userinfo answers 400 with {"error":"invalid_request","error_description":"Bearer token missing"} rather than the RFC 6750 401 with a WWW-Authenticate header.
  description: 'Qatar University''s own WSO2 OpenID Connect provider. Discovery, JWKS and the authorization, token, userinfo, introspection, revocation and logout endpoints are all published. Client authentication is client_secret_basic or client_secret_post; PKCE is supported with S256 and plain; subject_types is pairwise; ID tokens are RS256. Ten grant types are advertised, including the legacy `password` grant and WSO2''s non-standard `iwa:ntlm` and `account_switch`. A Dynamic Client Registration endpoint is advertised at /api/identity/oauth2/dcr/v1.1/register, but no public self-service onboarding for it was found: obtaining a client is an institutional process, not a developer signup. Scopes are the five OIDC standard scopes only — see scopes/qatar-scopes.yml.'
  evidence:
    status: 200
    url: https://sso.qu.edu.qa/oauth2/token/.well-known/openid-configuration
  name: QuSsoOpenIdConnect
  openIdConnectUrl: https://sso.qu.edu.qa/oauth2/token/.well-known/openid-configuration
  operator: institution
  type: openIdConnect
- applies_to: https://sso.qu.edu.qa/samlsso
  description: The same provider publishes a SAML 2.0 IDPSSODescriptor at /identity/metadata/saml2 with HTTP-POST and HTTP-Redirect SSO bindings and separate signing and encryption keys. Relying-party registration is institutional. The metadata declares no NameIDFormat and no Organization or ContactPerson element.
  evidence:
    status: 200
    url: https://sso.qu.edu.qa/identity/metadata/saml2
  name: QuSsoSaml2
  operator: institution
  type: saml
- applies_to: https://elearning.qu.edu.qa/learn/api/public/v1
  description: Qatar University's Blackboard Learn tenant exposes the Anthology Blackboard Learn REST API. /system/version is anonymous and answers 200 with the running build; every content route requires an OAuth 2.0 bearer token issued to a developer-registered application, and /courses answers 401 without one. The authentication model, the token endpoint and the contract are Anthology's, not Qatar University's — recorded here for completeness and scored against Blackboard.
  evidence:
  - status: 200
    url: https://elearning.qu.edu.qa/learn/api/public/v1/system/version
  - status: 401
    url: https://elearning.qu.edu.qa/learn/api/public/v1/courses
  name: BlackboardLearnRest
  operator: tenant
  type: oauth2
slug: qatar-authentication
source_filename: qatar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Evangelist Authentication\nspecificationVersion: '0.1'\nx-method: derived  # authorship, for build-provenance-manifest.py — API Evangelist wrote this file; see `method:` below for how the facts in it were obtained\nprovider: Qatar University\nproviderId: qatar\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes on 2026-09-01 of every surface attributed to Qatar University, with no\n  credential of any kind presented to any endpoint. Replaces no earlier file — the repository\n  held no authentication artifact before this run.\ndescription: >-\n  Qatar University's public programmable surfaces divide cleanly. Everything that harvests or\n  reads scholarly metadata is open and anonymous — the QU Press OJS OAI-PMH endpoint that the\n  university operates itself, and the QSpace repository endpoints that its hosting provider\n  operates for it. Everything that touches a person is behind the university's own OpenID\n  Connect / SAML provider at sso.qu.edu.qa,\
  \ and there is no public onboarding path to it.\n  No Qatar University surface issues API keys to the public, and none was found that documents\n  an authentication model in prose.\nsummary:\n  types:\n    - none\n    - oauth2\n    - openIdConnect\n    - saml\n  institution_operated_public_apis_requiring_no_auth: 1\n  tenant_operated_public_apis_requiring_no_auth: 3\n  public_self_service_credential_available: false\nschemes:\n  - name: QSpaceOaiPublic\n    type: none\n    operator: tenant\n    operator_basis: >-\n      qspace.qu.edu.qa CNAMEs to qataru.cname.openrepository.com and resolves to 3.255.61.143\n      (Amazon eu-west-1). Open Repository is a commercial hosted-DSpace service; the hostname,\n      content and Handle prefix are Qatar University's, the deployment is not.\n    applies_to: https://qspace.qu.edu.qa/server/oai/request\n    description: >-\n      OAI-PMH harvesting is fully anonymous. Identify, ListMetadataFormats, ListSets,\n      ListIdentifiers, ListRecords and GetRecord\
  \ all answer 200 with no credential and no\n      rate-limit header. The repository publishes no harvesting policy.\n    evidence:\n      url: 'https://qspace.qu.edu.qa/server/oai/request?verb=Identify'\n      status: 200\n  - name: QSpaceRestPublicRead\n    type: none\n    operator: tenant\n    applies_to: https://qspace.qu.edu.qa/server/api\n    description: >-\n      DSpace 7.6 read operations — the service root, communities, collections, items and\n      discovery search — are anonymous. Write operations require a DSpace account and a\n      CSRF token (DSpace's `DSPACE-XSRF-TOKEN` header exchange); no public registration\n      path was found, so the write half of the API is not reachable by the public.\n    evidence:\n      url: https://qspace.qu.edu.qa/server/api\n      status: 200\n  - name: QSpaceOpenSearchPublic\n    type: none\n    operator: tenant\n    applies_to: https://qspace.qu.edu.qa/server/opensearch\n    description: OpenSearch description and Atom/RSS result feeds are\
  \ anonymous.\n    evidence:\n      url: https://qspace.qu.edu.qa/server/opensearch/service\n      status: 200\n  - name: QuPressOaiPublic\n    type: none\n    operator: institution\n    applies_to: https://journals.qu.edu.qa/index.php/index/oai\n    description: >-\n      QU Press OJS OAI-PMH harvesting is anonymous over all nine journals. The adjacent OJS\n      REST API at /index.php/{journal}/api/v1/ is NOT public — it returns 403 to\n      unauthenticated callers, and OJS gates it behind an API token issued per user account.\n    evidence:\n      url: 'https://journals.qu.edu.qa/index.php/index/oai?verb=Identify'\n      status: 200\n  - name: QuSsoOpenIdConnect\n    type: openIdConnect\n    operator: institution\n    applies_to: https://sso.qu.edu.qa\n    openIdConnectUrl: https://sso.qu.edu.qa/oauth2/token/.well-known/openid-configuration\n    description: >-\n      Qatar University's own WSO2 OpenID Connect provider. Discovery, JWKS and the\n      authorization, token, userinfo,\
  \ introspection, revocation and logout endpoints are all\n      published. Client authentication is client_secret_basic or client_secret_post; PKCE is\n      supported with S256 and plain; subject_types is pairwise; ID tokens are RS256.\n      Ten grant types are advertised, including the legacy `password` grant and WSO2's\n      non-standard `iwa:ntlm` and `account_switch`.\n      A Dynamic Client Registration endpoint is advertised at\n      /api/identity/oauth2/dcr/v1.1/register, but no public self-service onboarding for it was\n      found: obtaining a client is an institutional process, not a developer signup.\n      Scopes are the five OIDC standard scopes only — see scopes/qatar-scopes.yml.\n    evidence:\n      url: https://sso.qu.edu.qa/oauth2/token/.well-known/openid-configuration\n      status: 200\n    caveats:\n      - >-\n        The discovery document is at a non-standard location. RFC 8414 says to append\n        /.well-known/openid-configuration to the issuer; here it\
  \ is nested under /oauth2/token/,\n        and the issuer itself (https://sso.qu.edu.qa:9443/oauth2endpoints/token) points at the\n        WSO2 management port. A conformant client discovering by the book will not find it.\n      - >-\n        The host serves an incomplete TLS chain, so a default OpenSSL-based client cannot read\n        the discovery document at all. See identity-federation/qatar-identity-federation.yml.\n      - >-\n        /oauth2/userinfo answers 400 with {\"error\":\"invalid_request\",\"error_description\":\"Bearer\n        token missing\"} rather than the RFC 6750 401 with a WWW-Authenticate header.\n  - name: QuSsoSaml2\n    type: saml\n    operator: institution\n    applies_to: https://sso.qu.edu.qa/samlsso\n    description: >-\n      The same provider publishes a SAML 2.0 IDPSSODescriptor at /identity/metadata/saml2\n      with HTTP-POST and HTTP-Redirect SSO bindings and separate signing and encryption keys.\n      Relying-party registration is institutional.\
  \ The metadata declares no NameIDFormat and\n      no Organization or ContactPerson element.\n    evidence:\n      url: https://sso.qu.edu.qa/identity/metadata/saml2\n      status: 200\n  - name: BlackboardLearnRest\n    type: oauth2\n    operator: tenant\n    applies_to: https://elearning.qu.edu.qa/learn/api/public/v1\n    description: >-\n      Qatar University's Blackboard Learn tenant exposes the Anthology Blackboard Learn REST\n      API. /system/version is anonymous and answers 200 with the running build; every\n      content route requires an OAuth 2.0 bearer token issued to a developer-registered\n      application, and /courses answers 401 without one. The authentication model, the token\n      endpoint and the contract are Anthology's, not Qatar University's — recorded here for\n      completeness and scored against Blackboard.\n    evidence:\n      - url: https://elearning.qu.edu.qa/learn/api/public/v1/system/version\n        status: 200\n      - url: https://elearning.qu.edu.qa/learn/api/public/v1/courses\n\
  \        status: 401\nnotes:\n  - >-\n    No Qatar University surface offers a public API key, developer account or self-service\n    credential. Where a credential is needed, the path is institutional affiliation.\n  - >-\n    An institutional API gateway exists but publishes nothing: api.qu.edu.qa resolves to\n    34.18.7.7 and answers 404 with a zero-length body and an F5 BIG-IP `BIGipServerPROD-API-POOL`\n    cookie. A production API pool is running behind it; no route, no documentation and no\n    authentication model for it is public.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qatar/refs/heads/main/authentication/qatar-authentication.yml
summary_line: none/oauth2/openIdConnect/saml · 7 schemes
tags:
- Education
- Higher Education
- University
- Qatar
- Middle East
- Research
- Identity Federation
- Scholarly Publishing
- Research Repository
- Open Access
- OAI-PMH
- SAML
- OpenID Connect
---
