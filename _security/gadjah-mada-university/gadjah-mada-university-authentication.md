---
api_key_in: []
api_specs:
- filename: gadjah-mada-university-ugm-id-openapi.yml
  format: yaml
  label: UGM ID — OAuth 2.0 / OpenID Connect Authorization Server
  slug: ugm-id
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-ugm-id-openapi.yml
- filename: gadjah-mada-university-repository-oai-pmh-openapi.yml
  format: yaml
  label: UGM Institutional Repository OAI-PMH
  slug: repository-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-repository-oai-pmh-openapi.yml
- filename: gadjah-mada-university-journal-oai-pmh-openapi.yml
  format: yaml
  label: UGM Journals OAI-PMH
  slug: journal-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-journal-oai-pmh-openapi.yml
auth_types:
- oauth2
- oidc
- saml2
- cas
description: ''
kind: authentication
layout: security
method: probed
name: Gadjah Mada University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gadjah Mada University secures its APIs with oauth2, oidc, saml2, and cas across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gadjah Mada University
provider_slug: gadjah-mada-university
scheme_count: 3
schemes:
- claims:
  - sub
  - iss
  - aud
  - exp
  - iat
  - auth_time
  - name
  - given_name
  - family_name
  - picture
  - email
  - email_verified
  - preferred_username
  - unit_id
  client_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  defects_observed:
  - defect: Both discovery documents emit scheme-less URLs. `issuer` is "oauth.simaster.ugm.ac.id" and every endpoint is "oauth.simaster.ugm.ac.id/oauth/..." rather than an absolute https:// URL. OIDC Discovery and RFC 8414 both require absolute URLs; a conforming client library will reject or mis-resolve these. Recorded as observed, not corrected.
    location: https://oauth.simaster.ugm.ac.id/.well-known/openid-configuration
    probed: '2026-09-01'
    status: 200
  - defect: https://oauth.simaster.ugm.ac.id/.well-known/jwks.json returns HTTP 200 with an EMPTY key set, {"keys":[]}. RS256 id_tokens are advertised but no public key is published, so no relying party can verify a token offline. The endpoint is documented in the OpenAPI as getJwks.
    location: https://oauth.simaster.ugm.ac.id/.well-known/jwks.json
    probed: '2026-09-01'
    status: 200
  - defect: The `password` (resource owner credentials) grant and `none` client authentication are both advertised. The OpenAPI's own description flags `none` as legacy and slated for removal.
    location: https://oauth.simaster.ugm.ac.id/openapi.json
    probed: '2026-09-01'
    status: 200
  description: UGM ID, the university's OAuth 2.0 / OpenID Connect authorization server, operated by DTI at oauth.simaster.ugm.ac.id. Issuer, endpoints, grants, scopes and claims are published in both an OIDC Discovery document and an RFC 8414 authorization server metadata document. The OpenAPI that describes it is written by UGM in Indonesian and is the institution's own contract.
  discovery:
  - https://oauth.simaster.ugm.ac.id/.well-known/openid-configuration
  - https://oauth.simaster.ugm.ac.id/.well-known/oauth-authorization-server
  endpoints:
    authorization: https://oauth.simaster.ugm.ac.id/oauth/authorize
    end_session: https://oauth.simaster.ugm.ac.id/oauth/logout
    introspection: https://oauth.simaster.ugm.ac.id/oauth/introspect
    jwks: https://oauth.simaster.ugm.ac.id/.well-known/jwks.json
    revocation: https://oauth.simaster.ugm.ac.id/oauth/revoke
    token: https://oauth.simaster.ugm.ac.id/oauth/token
    userinfo: https://oauth.simaster.ugm.ac.id/userinfo
  grant_types:
  - authorization_code
  - password
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:google_id_token
  - urn:ietf:params:oauth:grant-type:token-exchange
  id_token_signing_alg:
  - RS256
  issuer: oauth.simaster.ugm.ac.id
  name: ugm-id-oauth2-oidc
  onboarding:
    note: No client registration page, no dynamic client registration endpoint, and no published request process were found. Client credentials appear to be issued internally by DTI to UGM units. An outside developer has read access to the contract and to /health, and nothing else.
    self_service: false
  pkce:
    code_challenge_methods:
    - S256
    supported: true
  response_types:
  - code
  rfcs_implemented:
  - RFC 6749 (OAuth 2.0)
  - RFC 7009 (Token Revocation)
  - RFC 7636 (PKCE)
  - RFC 7662 (Token Introspection)
  - RFC 8414 (Authorization Server Metadata)
  - RFC 8693 (Token Exchange)
  - OpenID Connect Core + Discovery
  social_login:
  - google
  - microsoft
  - facebook
  - linkedin
  - apple
  type: oauth2
  x-operator: institution
- defects_observed:
  - defect: shibmd:Scope is declared as "ac.id" — the whole Indonesian academic second-level domain — rather than "ugm.ac.id". A scope that broad asserts authority over every Indonesian institution's namespace and would be rejected by a federation operator on registration.
    location: https://sso.ugm.ac.id/idp/shibboleth
    probed: '2026-09-01'
    status: 200
  - defect: The signing certificate in the descriptor was issued 2014-12-16 (valid to 2034-12-16), an 11-year-old key still in production use.
    location: authentication/gadjah-mada-university-saml-idp-metadata.xml
    probed: '2026-09-01'
    status: local
  - defect: The entity is NOT present in the eduGAIN metadata aggregate. The full eduGAIN entity list (10,616 entities, retrieved 2026-09-01) contains no ugm.ac.id entity, so the IdP is self-published only and not inter-federated.
    location: https://technical.edugain.org/api.php?action=list_entities&format=json
    probed: '2026-09-01'
    status: 200
  description: 'UGM''s own Shibboleth Identity Provider at sso.ugm.ac.id, publishing an unsigned SAML 2.0 EntityDescriptor from its own host. Advertises SAML 2.0, SAML 1.1 and the native Shibboleth authn profile, with an AttributeAuthorityDescriptor alongside the IDPSSODescriptor. This is institutional SSO infrastructure, not a developer API: an application cannot obtain an assertion without being registered as a service provider.'
  endpoints:
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
    location: https://sso.ugm.ac.id/idp/profile/SAML2/Redirect/SSO
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
    location: https://sso.ugm.ac.id/idp/profile/SAML2/POST/SSO
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign
    location: https://sso.ugm.ac.id/idp/profile/SAML2/POST-SimpleSign/SSO
  - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest
    location: https://sso.ugm.ac.id/idp/profile/Shibboleth/SSO
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP
    location: https://sso.ugm.ac.id/idp/profile/SAML2/SOAP/AttributeQuery
    role: AttributeAuthority
  entity_id: https://sso.ugm.ac.id/idp/shibboleth
  local_copy: authentication/gadjah-mada-university-saml-idp-metadata.xml
  metadata:
  - https://sso.ugm.ac.id/idp/shibboleth
  - https://sso.ugm.ac.id/idp/profile/Metadata/SAML
  name: ugm-shibboleth-saml2
  name_id_formats:
  - urn:mace:shibboleth:1.0:nameIdentifier
  - urn:oasis:names:tc:SAML:2.0:nameid-format:transient
  protocols:
  - urn:mace:shibboleth:1.0
  - urn:oasis:names:tc:SAML:1.1:protocol
  - urn:oasis:names:tc:SAML:2.0:protocol
  scope: ac.id
  single_logout:
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
  - urn:oasis:names:tc:SAML:2.0:bindings:SOAP
  type: saml2
  x-operator: institution
- description: Central Authentication Service at sso.ugm.ac.id/cas, the login surface UGM systems redirect to. A bare GET redirects to /cas/login and returns the login form. CAS is a ticket protocol with a machine-readable /serviceValidate response, but UGM publishes no service registration route and no protocol documentation, so it is recorded as an authentication surface rather than an API.
  endpoints:
    login: https://sso.ugm.ac.id/cas/login
  name: ugm-cas
  probed: '2026-09-01'
  status: 200
  type: cas
  x-operator: institution
slug: gadjah-mada-university-authentication
source_filename: gadjah-mada-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes on 2026-09-01 of Universitas Gadjah Mada's own authentication surfaces, plus the\n  institution's SAML entity descriptor retrieved directly from its Shibboleth IdP metadata\n  endpoint. Every scheme below is on a host under the ugm.ac.id registrable domain.\nx-operator: institution\n\nsummary:\n  note: >-\n    UGM is unusual for this cohort: it operates a real, first-party OAuth 2.0 / OpenID Connect\n    authorization server — UGM ID — with a published OpenAPI 3.1.0 document, RFC 8414 and OIDC\n    discovery documents, PKCE, token introspection (RFC 7662), token revocation (RFC 7009) and\n    RFC 8693 token exchange. It ALSO runs a Shibboleth SAML 2.0 Identity Provider and a CAS\n    server. Three separate institution-operated identity stacks, all self-hosted. What it does\n    not have is self-service developer onboarding: there is no public client registration, no\n    dynamic client registration endpoint,\
  \ and no documented route for an outside developer to\n    obtain a client_id. Credentials are issued internally by DTI.\n  types:\n  - oauth2\n  - oidc\n  - saml2\n  - cas\n  public_oauth: true\n  self_serve_api_keys: false\n  dynamic_client_registration: false\n\nschemes:\n\n- name: ugm-id-oauth2-oidc\n  type: oauth2\n  x-operator: institution\n  description: >-\n    UGM ID, the university's OAuth 2.0 / OpenID Connect authorization server, operated by DTI at\n    oauth.simaster.ugm.ac.id. Issuer, endpoints, grants, scopes and claims are published in both an\n    OIDC Discovery document and an RFC 8414 authorization server metadata document. The OpenAPI\n    that describes it is written by UGM in Indonesian and is the institution's own contract.\n  issuer: oauth.simaster.ugm.ac.id\n  discovery:\n  - https://oauth.simaster.ugm.ac.id/.well-known/openid-configuration\n  - https://oauth.simaster.ugm.ac.id/.well-known/oauth-authorization-server\n  endpoints:\n    authorization: https://oauth.simaster.ugm.ac.id/oauth/authorize\n\
  \    token: https://oauth.simaster.ugm.ac.id/oauth/token\n    introspection: https://oauth.simaster.ugm.ac.id/oauth/introspect\n    revocation: https://oauth.simaster.ugm.ac.id/oauth/revoke\n    userinfo: https://oauth.simaster.ugm.ac.id/userinfo\n    end_session: https://oauth.simaster.ugm.ac.id/oauth/logout\n    jwks: https://oauth.simaster.ugm.ac.id/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - password\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:google_id_token\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  pkce:\n    supported: true\n    code_challenge_methods: [S256]\n  client_auth_methods: [client_secret_basic, client_secret_post, none]\n  id_token_signing_alg: [RS256]\n  response_types: [code]\n  claims:\n  - sub\n  - iss\n  - aud\n  - exp\n  - iat\n  - auth_time\n  - name\n  - given_name\n  - family_name\n  - picture\n  - email\n  - email_verified\n  - preferred_username\n  - unit_id\n  social_login:\n  - google\n\
  \  - microsoft\n  - facebook\n  - linkedin\n  - apple\n  rfcs_implemented:\n  - RFC 6749 (OAuth 2.0)\n  - RFC 7009 (Token Revocation)\n  - RFC 7636 (PKCE)\n  - RFC 7662 (Token Introspection)\n  - RFC 8414 (Authorization Server Metadata)\n  - RFC 8693 (Token Exchange)\n  - OpenID Connect Core + Discovery\n  defects_observed:\n  - defect: >-\n      Both discovery documents emit scheme-less URLs. `issuer` is \"oauth.simaster.ugm.ac.id\" and\n      every endpoint is \"oauth.simaster.ugm.ac.id/oauth/...\" rather than an absolute https:// URL.\n      OIDC Discovery and RFC 8414 both require absolute URLs; a conforming client library will\n      reject or mis-resolve these. Recorded as observed, not corrected.\n    probed: '2026-09-01'\n    location: https://oauth.simaster.ugm.ac.id/.well-known/openid-configuration\n    status: 200\n  - defect: >-\n      https://oauth.simaster.ugm.ac.id/.well-known/jwks.json returns HTTP 200 with an EMPTY key set,\n      {\"keys\":[]}. RS256 id_tokens are advertised\
  \ but no public key is published, so no relying\n      party can verify a token offline. The endpoint is documented in the OpenAPI as getJwks.\n    probed: '2026-09-01'\n    location: https://oauth.simaster.ugm.ac.id/.well-known/jwks.json\n    status: 200\n  - defect: >-\n      The `password` (resource owner credentials) grant and `none` client authentication are both\n      advertised. The OpenAPI's own description flags `none` as legacy and slated for removal.\n    probed: '2026-09-01'\n    location: https://oauth.simaster.ugm.ac.id/openapi.json\n    status: 200\n  onboarding:\n    self_service: false\n    note: >-\n      No client registration page, no dynamic client registration endpoint, and no published\n      request process were found. Client credentials appear to be issued internally by DTI to UGM\n      units. An outside developer has read access to the contract and to /health, and nothing else.\n\n- name: ugm-shibboleth-saml2\n  type: saml2\n  x-operator: institution\n  description:\
  \ >-\n    UGM's own Shibboleth Identity Provider at sso.ugm.ac.id, publishing an unsigned SAML 2.0\n    EntityDescriptor from its own host. Advertises SAML 2.0, SAML 1.1 and the native Shibboleth\n    authn profile, with an AttributeAuthorityDescriptor alongside the IDPSSODescriptor. This is\n    institutional SSO infrastructure, not a developer API: an application cannot obtain an\n    assertion without being registered as a service provider.\n  entity_id: https://sso.ugm.ac.id/idp/shibboleth\n  metadata:\n  - https://sso.ugm.ac.id/idp/shibboleth\n  - https://sso.ugm.ac.id/idp/profile/Metadata/SAML\n  local_copy: authentication/gadjah-mada-university-saml-idp-metadata.xml\n  scope: ac.id\n  protocols:\n  - urn:mace:shibboleth:1.0\n  - urn:oasis:names:tc:SAML:1.1:protocol\n  - urn:oasis:names:tc:SAML:2.0:protocol\n  endpoints:\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    location: https://sso.ugm.ac.id/idp/profile/SAML2/Redirect/SSO\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n\
  \    location: https://sso.ugm.ac.id/idp/profile/SAML2/POST/SSO\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n    location: https://sso.ugm.ac.id/idp/profile/SAML2/POST-SimpleSign/SSO\n  - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest\n    location: https://sso.ugm.ac.id/idp/profile/Shibboleth/SSO\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n    location: https://sso.ugm.ac.id/idp/profile/SAML2/SOAP/AttributeQuery\n    role: AttributeAuthority\n  name_id_formats:\n  - urn:mace:shibboleth:1.0:nameIdentifier\n  - urn:oasis:names:tc:SAML:2.0:nameid-format:transient\n  single_logout:\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n  - urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n  defects_observed:\n  - defect: >-\n      shibmd:Scope is declared as \"ac.id\" — the whole Indonesian academic second-level domain —\n      rather than \"ugm.ac.id\". A scope that broad asserts authority over\
  \ every Indonesian\n      institution's namespace and would be rejected by a federation operator on registration.\n    probed: '2026-09-01'\n    location: https://sso.ugm.ac.id/idp/shibboleth\n    status: 200\n  - defect: >-\n      The signing certificate in the descriptor was issued 2014-12-16 (valid to 2034-12-16), an\n      11-year-old key still in production use.\n    probed: '2026-09-01'\n    location: authentication/gadjah-mada-university-saml-idp-metadata.xml\n    status: local\n  - defect: >-\n      The entity is NOT present in the eduGAIN metadata aggregate. The full eduGAIN entity list\n      (10,616 entities, retrieved 2026-09-01) contains no ugm.ac.id entity, so the IdP is\n      self-published only and not inter-federated.\n    probed: '2026-09-01'\n    location: https://technical.edugain.org/api.php?action=list_entities&format=json\n    status: 200\n\n- name: ugm-cas\n  type: cas\n  x-operator: institution\n  description: >-\n    Central Authentication Service at sso.ugm.ac.id/cas,\
  \ the login surface UGM systems redirect to.\n    A bare GET redirects to /cas/login and returns the login form. CAS is a ticket protocol with a\n    machine-readable /serviceValidate response, but UGM publishes no service registration route and\n    no protocol documentation, so it is recorded as an authentication surface rather than an API.\n  endpoints:\n    login: https://sso.ugm.ac.id/cas/login\n  probed: '2026-09-01'\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/authentication/gadjah-mada-university-authentication.yml
summary_line: oauth2/oidc/saml2/cas · 3 schemes
tags:
- University
- Higher Education
- Education
- Indonesia
- Research
- Identity Federation
- Authentication
- OpenID Connect
- OAuth
- Research Repository
- Scholarly Publishing
- OAI-PMH
- Library
---
