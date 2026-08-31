---
api_key_in: []
api_specs:
- filename: columbia-locations-api-openapi.yml
  format: yaml
  label: Columbia University Locations API
  slug: columbia-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/columbia/refs/heads/main/openapi/columbia-locations-api-openapi.yml
auth_types: []
description: 'How authentication works across the surfaces Columbia University operates. The shape of this file is the shape of the institution: one small API that needs no credential at all, and an otherwise complete estate that is reachable only with a Columbia UNI. There is no API key, no OAuth client registration, no developer account and no self-service path to any Columbia surface for a caller who is not affiliated with the university.'
kind: authentication
layout: security
method: probed
name: Columbia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Columbia University declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Columbia University
provider_slug: columbia
scheme_count: 6
schemes:
- applies_to:
  - Columbia University Libraries Hours API (hours.library.columbia.edu/api/v1)
  - Columbia Shibboleth IdP metadata (shibboleth.columbia.edu/idp/shibboleth)
  - CLIO catalogue MARCXML bulk extracts (lito.cul.columbia.edu)
  - CU Directory of Classes (doc.sis.columbia.edu)
  description: 'No credential of any kind. The Hours API explicitly skips authentication for its two public operations — Columbia''s own source carries `skip_before_action :authenticate_user!, only: [:open_hours, :open_now]` — and sets Access-Control-Allow-Origin: * on both, making it directly callable from a browser or an agent with no key exchange.'
  evidence: https://hours.library.columbia.edu/api/v1/locations/open_now
  id: none
  method: probed
  name: Anonymous
  status_code: 200
  x-operator: institution
- applies_to:
  - Columbia Open Data Service data feeds (opendataservice.columbia.edu)
  - Columbia web applications generally
  description: 'Columbia University Information Technology operates a CAS server at cas.columbia.edu for browser-based single sign-on with UNI credentials and multi-factor authentication. It is a human login flow, not an API credential: there is no token endpoint a non-browser client can call and no way for an unaffiliated developer to obtain a UNI. CAS also terminates the Shibboleth IdP''s SingleLogoutService.'
  evidence: https://cas.columbia.edu/cas/login
  id: cas
  method: probed
  name: Columbia CAS (Central Authentication Service)
  status_code: 200
  type: browser_sso
  x-operator: institution
- applies_to:
  - Federated web applications integrated by CUIT
  - InCommon and eduGAIN service providers
  artifact: examples/columbia-shibboleth-idp-metadata-example.xml
  description: Columbia runs its own production Shibboleth IdP and publishes signed SAML 2.0 metadata anonymously. Relying parties are registered by CUIT; there is no public or dynamic service provider registration, so an unaffiliated party cannot integrate. Supports SAML 2.0, SAML 1.1 and Shibboleth 1.0 protocols across HTTP-Redirect, HTTP-POST and HTTP-POST-SimpleSign bindings. Scope is columbia.edu.
  endpoints:
    metadata: https://shibboleth.columbia.edu/idp/shibboleth
    slo: https://cas.columbia.edu/cas/logout
    sso_post: https://shibboleth.columbia.edu/idp/profile/SAML2/POST/SSO
    sso_post_simplesign: https://shibboleth.columbia.edu/idp/profile/SAML2/POST-SimpleSign/SSO
    sso_redirect: https://shibboleth.columbia.edu/idp/profile/SAML2/Redirect/SSO
    sso_shibboleth: https://shibboleth.columbia.edu/idp/profile/Shibboleth/SSO
  entity_id: urn:mace:incommon:columbia.edu
  evidence: https://shibboleth.columbia.edu/idp/shibboleth
  id: shibboleth-saml
  method: probed
  name: Columbia Shibboleth Identity Provider (SAML 2.0)
  status_code: 200
  type: saml
  x-operator: institution
- applies_to:
  - Columbia Open Data Service (opendataservice.columbia.edu)
  description: 'The Open Data Service — the closest thing Columbia has to a developer portal, publishing JSON and XML feeds for the course directory, the CLIO catalogue and building access — states that any member of the University community may log in with their UNI to consume the feeds. That is the whole access model: affiliation is the credential. There is no external tier, no partner tier and no application process for a non-Columbia caller.'
  evidence: https://opendataservice.columbia.edu/about
  id: uni-login
  method: searched
  name: Columbia UNI affiliation gate
  note: The Open Data Service is behind a Cloudflare managed challenge and its documentation could not be read directly on this run. The access model above is carried forward from the prior profile and is not re-verified; it is not upgraded to `probed`.
  status_code: 403
  type: affiliation_gated
  x-operator: institution
- description: Columbia's Shibboleth IdP does not publish an OIDC discovery document. shibboleth.columbia.edu/.well-known/openid-configuration returns 404 and /idp/profile/oidc/keyset returns HTTP 500. The identity estate is SAML-only in everything it publishes.
  evidence: https://shibboleth.columbia.edu/.well-known/openid-configuration
  id: oidc-absent
  method: probed
  name: OpenID Connect
  status: not_published
  status_code: 404
  x-operator: institution
- description: CourseWorks, Columbia's learning management system, is Instructure's Canvas. Its REST API accepts Canvas access tokens issued to Columbia accounts and returns a structured JSON 401 otherwise. The credential, the token lifecycle and the documentation are Instructure's; Columbia supplies the users.
  evidence: https://courseworks2.columbia.edu/api/v1/accounts
  id: canvas-token
  method: probed
  name: Instructure Canvas bearer token (CourseWorks)
  status_code: 401
  type: bearer
  x-operator: tenant
slug: columbia-authentication
source_filename: columbia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  Live probes of Columbia University identity and API hosts on 2026-08-19, plus Columbia's\n  published Shibboleth IdP metadata and the CUIT web authentication documentation pointer.\nprovider: Columbia University\nproviderId: columbia\ndescription: >-\n  How authentication works across the surfaces Columbia University operates. The shape of this\n  file is the shape of the institution: one small API that needs no credential at all, and an\n  otherwise complete estate that is reachable only with a Columbia UNI. There is no API key, no\n  OAuth client registration, no developer account and no self-service path to any Columbia\n  surface for a caller who is not affiliated with the university.\nschemes:\n- id: none\n  name: Anonymous\n  x-operator: institution\n  applies_to:\n  - Columbia University Libraries Hours API (hours.library.columbia.edu/api/v1)\n  - Columbia Shibboleth IdP metadata (shibboleth.columbia.edu/idp/shibboleth)\n\
  \  - CLIO catalogue MARCXML bulk extracts (lito.cul.columbia.edu)\n  - CU Directory of Classes (doc.sis.columbia.edu)\n  description: >-\n    No credential of any kind. The Hours API explicitly skips authentication for its two public\n    operations — Columbia's own source carries `skip_before_action :authenticate_user!, only:\n    [:open_hours, :open_now]` — and sets Access-Control-Allow-Origin: * on both, making it\n    directly callable from a browser or an agent with no key exchange.\n  method: probed\n  evidence: https://hours.library.columbia.edu/api/v1/locations/open_now\n  status_code: 200\n- id: cas\n  name: Columbia CAS (Central Authentication Service)\n  type: browser_sso\n  x-operator: institution\n  applies_to:\n  - Columbia Open Data Service data feeds (opendataservice.columbia.edu)\n  - Columbia web applications generally\n  description: >-\n    Columbia University Information Technology operates a CAS server at cas.columbia.edu for\n    browser-based single sign-on with\
  \ UNI credentials and multi-factor authentication. It is a\n    human login flow, not an API credential: there is no token endpoint a non-browser client can\n    call and no way for an unaffiliated developer to obtain a UNI. CAS also terminates the\n    Shibboleth IdP's SingleLogoutService.\n  method: probed\n  evidence: https://cas.columbia.edu/cas/login\n  status_code: 200\n- id: shibboleth-saml\n  name: Columbia Shibboleth Identity Provider (SAML 2.0)\n  type: saml\n  x-operator: institution\n  entity_id: urn:mace:incommon:columbia.edu\n  applies_to:\n  - Federated web applications integrated by CUIT\n  - InCommon and eduGAIN service providers\n  description: >-\n    Columbia runs its own production Shibboleth IdP and publishes signed SAML 2.0 metadata\n    anonymously. Relying parties are registered by CUIT; there is no public or dynamic service\n    provider registration, so an unaffiliated party cannot integrate. Supports SAML 2.0, SAML 1.1\n    and Shibboleth 1.0 protocols across\
  \ HTTP-Redirect, HTTP-POST and HTTP-POST-SimpleSign\n    bindings. Scope is columbia.edu.\n  endpoints:\n    metadata: https://shibboleth.columbia.edu/idp/shibboleth\n    sso_redirect: https://shibboleth.columbia.edu/idp/profile/SAML2/Redirect/SSO\n    sso_post: https://shibboleth.columbia.edu/idp/profile/SAML2/POST/SSO\n    sso_post_simplesign: https://shibboleth.columbia.edu/idp/profile/SAML2/POST-SimpleSign/SSO\n    sso_shibboleth: https://shibboleth.columbia.edu/idp/profile/Shibboleth/SSO\n    slo: https://cas.columbia.edu/cas/logout\n  method: probed\n  evidence: https://shibboleth.columbia.edu/idp/shibboleth\n  status_code: 200\n  artifact: examples/columbia-shibboleth-idp-metadata-example.xml\n- id: uni-login\n  name: Columbia UNI affiliation gate\n  type: affiliation_gated\n  x-operator: institution\n  applies_to:\n  - Columbia Open Data Service (opendataservice.columbia.edu)\n  description: >-\n    The Open Data Service — the closest thing Columbia has to a developer portal, publishing\n\
  \    JSON and XML feeds for the course directory, the CLIO catalogue and building access — states\n    that any member of the University community may log in with their UNI to consume the feeds.\n    That is the whole access model: affiliation is the credential. There is no external tier, no\n    partner tier and no application process for a non-Columbia caller.\n  method: searched\n  evidence: https://opendataservice.columbia.edu/about\n  status_code: 403\n  note: >-\n    The Open Data Service is behind a Cloudflare managed challenge and its documentation could not\n    be read directly on this run. The access model above is carried forward from the prior profile\n    and is not re-verified; it is not upgraded to `probed`.\n- id: oidc-absent\n  name: OpenID Connect\n  status: not_published\n  x-operator: institution\n  description: >-\n    Columbia's Shibboleth IdP does not publish an OIDC discovery document.\n    shibboleth.columbia.edu/.well-known/openid-configuration returns 404 and\n\
  \    /idp/profile/oidc/keyset returns HTTP 500. The identity estate is SAML-only in everything it\n    publishes.\n  method: probed\n  evidence: https://shibboleth.columbia.edu/.well-known/openid-configuration\n  status_code: 404\n- id: canvas-token\n  name: Instructure Canvas bearer token (CourseWorks)\n  type: bearer\n  x-operator: tenant\n  description: >-\n    CourseWorks, Columbia's learning management system, is Instructure's Canvas. Its REST API\n    accepts Canvas access tokens issued to Columbia accounts and returns a structured JSON 401\n    otherwise. The credential, the token lifecycle and the documentation are Instructure's;\n    Columbia supplies the users.\n  method: probed\n  evidence: https://courseworks2.columbia.edu/api/v1/accounts\n  status_code: 401\nsummary:\n  public_no_auth_surfaces: 4\n  affiliation_gated_surfaces: 2\n  self_service_registration: false\n  api_keys_issued: false\n  oauth_client_registration: false\nnotes: >-\n  The honest headline is that Columbia\
  \ issues no API credential to anyone outside the university.\n  What saves the profile from being entirely gated is that the four surfaces which are open —\n  the Hours API, the IdP metadata, the CC0 MARCXML bulk extracts and the class directory — are\n  open completely, with no key, no quota and no click-through.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/columbia/refs/heads/main/authentication/columbia-authentication.yml
summary_line: 6 schemes
tags:
- University
- Higher Education
- Education
- Ivy League
- Private Research University
- United States
- New York
- Identity Federation
- Library
- Open Data
- Research Repository
- Research Data
- Course Catalog
- Campus Life
---
