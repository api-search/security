---
api_key_in: []
api_specs:
- filename: university-of-waikato-uowidp-openapi.yml
  format: yaml
  label: University of Waikato Identity Provider (uowidp)
  slug: uowidp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waikato/refs/heads/main/openapi/university-of-waikato-uowidp-openapi.yml
auth_types:
- openIdConnect
- http
- saml2
description: How authentication actually works across the University of Waikato's programmable surfaces. The institution runs one OpenID Connect provider of its own, fronting its Microsoft Entra ID tenant; federated access to external research and library services goes through SAML 2.0 in Tuakiri, the New Zealand Access Federation; and the two small service APIs on institution hosts each carry their own scheme. There is no self-serve developer credential anywhere on this estate.
kind: authentication
layout: security
method: probed
name: University Of Waikato Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Waikato secures its APIs with openIdConnect, http, and saml2 across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Waikato
provider_slug: university-of-waikato
scheme_count: 6
schemes:
- authorization_endpoint: https://api.svc.waikato.ac.nz/uowidp/v1/auth
  claims:
  - iss
  - aud
  - nbf
  - exp
  - iat
  - nonce
  - Username
  - name
  - ver
  - oid
  - sub
  end_session_endpoint: https://api.svc.waikato.ac.nz/uowidp/v1/logout
  grant_types:
  - authorization_code
  id_token_signing_alg:
  - RS256
  issuer: https://api.svc.waikato.ac.nz/uowidp/v1
  jwks_uri: https://api.svc.waikato.ac.nz/uowidp/v1/oidc/keys
  name: uowidp
  notes: Client registration is closed. The discovery document declares no registration_endpoint and no dynamic client registration; a client_id is issued by University of Waikato ITS. The provider is a facade over the university's Entra ID tenant 220f5dc3-9452-48e5-9b4f-888df42f7a2d — the userinfo endpoint is Microsoft Graph and the claim set (oid, ver) is Entra's.
  observed_clients:
  - client_id: timetable-prod
    evidence: https://timetable.waikato.ac.nz/appsettings.json
    for: https://timetable.waikato.ac.nz/ (ITS-built Blazor WebAssembly timetable)
  - client_id: SITS-Prod
    evidence: live authorization redirect observed 2026-09-01
    for: https://my.waikato.ac.nz/ (MyWaikato, Tribal SITS:Vision student portal)
  openIdConnectUrl: https://api.svc.waikato.ac.nz/uowidp/v1/.well-known/openid-configuration
  operator: institution
  response_modes:
  - query
  - fragment
  - form_post
  response_types:
  - code
  - id_token
  - code id_token
  scopes:
  - openid
  - profile
  - email
  token_endpoint: https://api.svc.waikato.ac.nz/uowidp/v1/token
  token_endpoint_auth_methods:
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://graph.microsoft.com/v1.0/me
  verified:
  - status: 200
    url: https://api.svc.waikato.ac.nz/uowidp/v1/.well-known/openid-configuration
  - status: 200
    url: https://api.svc.waikato.ac.nz/uowidp/v1/oidc/keys
  - status: 401
    url: https://api.svc.waikato.ac.nz/uowidp/v1/auth
  - status: 302
    url: https://api.svc.waikato.ac.nz/uowidp/v1/logout
- assurance:
  - https://refeds.org/sirtfi
  entity_categories:
  - http://refeds.org/category/research-and-scholarship
  entity_id: https://idp.waikato.ac.nz/idp/shibboleth
  federation: Tuakiri — New Zealand Access Federation (REANNZ)
  name: tuakiri-saml
  notes: The entity, the users and the attribute release are the institution's; the IdP deployment runs on REANNZ's Tuakiri Hosted IdP service. Exported to eduGAIN.
  operator: federation
  registered: '2012-10-15'
  registration_authority: https://tuakiri.ac.nz/
  scope: waikato.ac.nz
  sso_locations:
  - https://hosted-login.tuakiri.ac.nz/hosting/waikato.ac.nz/idp/profile/SAML2/POST/SSO
  - https://hosted-login.tuakiri.ac.nz/hosting/waikato.ac.nz/idp/profile/SAML2/Redirect/SSO
  type: saml2
  verified:
  - status: 200
    url: https://directory.tuakiri.ac.nz/metadata/tuakiri-metadata-signed.xml
  - status: 200
    url: https://mds.edugain.org/edugain-v2.xml
- issuer: https://login.microsoftonline.com/220f5dc3-9452-48e5-9b4f-888df42f7a2d/v2.0
  metadata: https://login.microsoftonline.com/220f5dc3-9452-48e5-9b4f-888df42f7a2d/federationmetadata/2007-06/federationmetadata.xml
  name: entra-saml
  notes: The university's Microsoft Entra ID tenant is the live SAML issuer for elearn.waikato.ac.nz and the identity source behind uowidp. Tenant region OC (Oceania), cloud microsoftonline.com.
  operator: federation
  tenant_id: 220f5dc3-9452-48e5-9b4f-888df42f7a2d
  type: saml2
  verified:
  - status: 200
    url: https://login.microsoftonline.com/220f5dc3-9452-48e5-9b4f-888df42f7a2d/v2.0/.well-known/openid-configuration
- description: The One-Time Secret service at otis.its.waikato.ac.nz authenticates every API request with HTTP Basic — username is the caller's Stella account login, password is an API token shown on the caller's account page. Credentials are institutional; there is no public sign-up.
  docs: https://otis.its.waikato.ac.nz/docs/api
  name: ots-basic
  operator: institution
  scheme: basic
  type: http
  verified:
  - status: 200
    url: https://otis.its.waikato.ac.nz/docs/api
- description: LTI 1.3 tool launches against the eLearn Moodle platform use signed JWT client credentials against the platform token endpoint, with the platform's public keys served from certs.php. Tool registration is by arrangement with the institution.
  grant_types:
  - client_credentials
  jwks_uri: https://elearn.waikato.ac.nz/mod/lti/certs.php
  name: lti-1p3-client-credentials
  operator: institution
  token_endpoint: https://elearn.waikato.ac.nz/mod/lti/token.php
  type: oauth2
  verified:
  - status: 200
    url: https://elearn.waikato.ac.nz/mod/lti/certs.php
- description: Research Commons serves its DSpace 7.6.5 REST API and OAI-PMH interface anonymously for read access; /server/api/authn is advertised for authenticated operations, which require a repository account.
  name: dspace-anonymous
  operator: institution
  type: none
  verified:
  - status: 200
    url: https://researchcommons.waikato.ac.nz/server/api
slug: university-of-waikato-authentication
source_filename: university-of-waikato-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  https://api.svc.waikato.ac.nz/uowidp/v1/.well-known/openid-configuration,\n  https://api.svc.waikato.ac.nz/uowidp/v1/oidc/keys,\n  https://timetable.waikato.ac.nz/appsettings.json,\n  https://otis.its.waikato.ac.nz/docs/api,\n  https://directory.tuakiri.ac.nz/metadata/tuakiri-metadata-signed.xml\ndescription: >-\n  How authentication actually works across the University of Waikato's programmable surfaces. The\n  institution runs one OpenID Connect provider of its own, fronting its Microsoft Entra ID tenant;\n  federated access to external research and library services goes through SAML 2.0 in Tuakiri, the\n  New Zealand Access Federation; and the two small service APIs on institution hosts each carry\n  their own scheme. There is no self-serve developer credential anywhere on this estate.\nsummary:\n  types: [openIdConnect, http, saml2]\n  self_serve_credentials: false\n  dynamic_client_registration: false\n  public_client_registration_endpoint:\
  \ none\nschemes:\n- name: uowidp\n  type: openIdConnect\n  operator: institution\n  issuer: https://api.svc.waikato.ac.nz/uowidp/v1\n  openIdConnectUrl: https://api.svc.waikato.ac.nz/uowidp/v1/.well-known/openid-configuration\n  jwks_uri: https://api.svc.waikato.ac.nz/uowidp/v1/oidc/keys\n  authorization_endpoint: https://api.svc.waikato.ac.nz/uowidp/v1/auth\n  token_endpoint: https://api.svc.waikato.ac.nz/uowidp/v1/token\n  end_session_endpoint: https://api.svc.waikato.ac.nz/uowidp/v1/logout\n  userinfo_endpoint: https://graph.microsoft.com/v1.0/me\n  grant_types: [authorization_code]\n  response_types: [code, id_token, code id_token]\n  response_modes: [query, fragment, form_post]\n  token_endpoint_auth_methods: [client_secret_post]\n  id_token_signing_alg: [RS256]\n  scopes: [openid, profile, email]\n  claims: [iss, aud, nbf, exp, iat, nonce, Username, name, ver, oid, sub]\n  observed_clients:\n  - client_id: timetable-prod\n    for: https://timetable.waikato.ac.nz/ (ITS-built Blazor\
  \ WebAssembly timetable)\n    evidence: https://timetable.waikato.ac.nz/appsettings.json\n  - client_id: SITS-Prod\n    for: https://my.waikato.ac.nz/ (MyWaikato, Tribal SITS:Vision student portal)\n    evidence: live authorization redirect observed 2026-09-01\n  notes: >-\n    Client registration is closed. The discovery document declares no registration_endpoint and no\n    dynamic client registration; a client_id is issued by University of Waikato ITS. The provider\n    is a facade over the university's Entra ID tenant 220f5dc3-9452-48e5-9b4f-888df42f7a2d — the\n    userinfo endpoint is Microsoft Graph and the claim set (oid, ver) is Entra's.\n  verified:\n  - url: https://api.svc.waikato.ac.nz/uowidp/v1/.well-known/openid-configuration\n    status: 200\n  - url: https://api.svc.waikato.ac.nz/uowidp/v1/oidc/keys\n    status: 200\n  - url: https://api.svc.waikato.ac.nz/uowidp/v1/auth\n    status: 401\n  - url: https://api.svc.waikato.ac.nz/uowidp/v1/logout\n    status: 302\n- name: tuakiri-saml\n\
  \  type: saml2\n  operator: federation\n  entity_id: https://idp.waikato.ac.nz/idp/shibboleth\n  federation: Tuakiri — New Zealand Access Federation (REANNZ)\n  registration_authority: https://tuakiri.ac.nz/\n  registered: '2012-10-15'\n  entity_categories: [http://refeds.org/category/research-and-scholarship]\n  assurance: [https://refeds.org/sirtfi]\n  scope: waikato.ac.nz\n  sso_locations:\n  - https://hosted-login.tuakiri.ac.nz/hosting/waikato.ac.nz/idp/profile/SAML2/POST/SSO\n  - https://hosted-login.tuakiri.ac.nz/hosting/waikato.ac.nz/idp/profile/SAML2/Redirect/SSO\n  notes: >-\n    The entity, the users and the attribute release are the institution's; the IdP deployment runs\n    on REANNZ's Tuakiri Hosted IdP service. Exported to eduGAIN.\n  verified:\n  - url: https://directory.tuakiri.ac.nz/metadata/tuakiri-metadata-signed.xml\n    status: 200\n  - url: https://mds.edugain.org/edugain-v2.xml\n    status: 200\n- name: entra-saml\n  type: saml2\n  operator: federation\n  tenant_id:\
  \ 220f5dc3-9452-48e5-9b4f-888df42f7a2d\n  issuer: https://login.microsoftonline.com/220f5dc3-9452-48e5-9b4f-888df42f7a2d/v2.0\n  metadata: https://login.microsoftonline.com/220f5dc3-9452-48e5-9b4f-888df42f7a2d/federationmetadata/2007-06/federationmetadata.xml\n  notes: >-\n    The university's Microsoft Entra ID tenant is the live SAML issuer for elearn.waikato.ac.nz and\n    the identity source behind uowidp. Tenant region OC (Oceania), cloud microsoftonline.com.\n  verified:\n  - url: https://login.microsoftonline.com/220f5dc3-9452-48e5-9b4f-888df42f7a2d/v2.0/.well-known/openid-configuration\n    status: 200\n- name: ots-basic\n  type: http\n  scheme: basic\n  operator: institution\n  description: >-\n    The One-Time Secret service at otis.its.waikato.ac.nz authenticates every API request with HTTP\n    Basic — username is the caller's Stella account login, password is an API token shown on the\n    caller's account page. Credentials are institutional; there is no public sign-up.\n\
  \  docs: https://otis.its.waikato.ac.nz/docs/api\n  verified:\n  - url: https://otis.its.waikato.ac.nz/docs/api\n    status: 200\n- name: lti-1p3-client-credentials\n  type: oauth2\n  grant_types: [client_credentials]\n  operator: institution\n  token_endpoint: https://elearn.waikato.ac.nz/mod/lti/token.php\n  jwks_uri: https://elearn.waikato.ac.nz/mod/lti/certs.php\n  description: >-\n    LTI 1.3 tool launches against the eLearn Moodle platform use signed JWT client credentials\n    against the platform token endpoint, with the platform's public keys served from certs.php.\n    Tool registration is by arrangement with the institution.\n  verified:\n  - url: https://elearn.waikato.ac.nz/mod/lti/certs.php\n    status: 200\n- name: dspace-anonymous\n  type: none\n  operator: institution\n  description: >-\n    Research Commons serves its DSpace 7.6.5 REST API and OAI-PMH interface anonymously for read\n    access; /server/api/authn is advertised for authenticated operations, which require\
  \ a\n    repository account.\n  verified:\n  - url: https://researchcommons.waikato.ac.nz/server/api\n    status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-waikato/refs/heads/main/authentication/university-of-waikato-authentication.yml
summary_line: openIdConnect/http/saml2 · 6 schemes
tags:
- Education
- Higher Education
- University
- New Zealand
- Research
- Research Repository
- Open Access
- OAI-PMH
- Identity Federation
- SAML
- OpenID Connect
- Learning Management
- Machine Learning
---
