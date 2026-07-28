---
api_key_in: []
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Nerc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: NERC secures its APIs with none, oauth2, and openIdConnect across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: NERC
provider_slug: nerc
scheme_count: 0
schemes: []
slug: nerc-authentication
source_filename: nerc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  Live probes of NERC-operated hosts on 2026-07-27, plus the E-ISAC OpenID\n  Connect discovery document at\n  https://www.eisac.com/.well-known/openid-configuration\nnote: >-\n  NERC publishes no developer API, so there is no OpenAPI securitySchemes block\n  to derive from. This profile is probed rather than derived, and it records what\n  a client actually meets on each NERC-operated surface. The headline: NERC's own\n  corporate estate has no programmatic authentication at all, while the one\n  standards-based auth surface in the whole estate belongs to E-ISAC and is\n  Salesforce Experience Cloud's stock OAuth2/OIDC issuer, gated to vetted\n  members.\nsummary:\n  types:\n  - none\n  - oauth2\n  - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  developer_signup: false\n  api_keys_issued: false\nsurfaces:\n- name: www.nerc.com public web and assets\n  host: https://www.nerc.com\n\
  \  auth: none\n  note: >-\n    Reliability Standards, reliability assessments, GADS/TADS statistical\n    brochures, the Compliance Registry Matrix XLSX and every /globalassets/*\n    document download anonymously over plain HTTPS GET. No key, no header, no\n    cookie.\n- name: Optimizely CMS site-search endpoints (undocumented)\n  host: https://www.nerc.com\n  paths:\n  - /api/search\n  - /api/search/events\n  - /api/search/news\n  - /api/search/terms\n  auth: none\n  documented: false\n  note: >-\n    Internal XHR routes of the Optimizely (Episerver) CMS that renders\n    nerc.com's own search UI, discovered from the site's JavaScript bundle and\n    re-verified live on 2026-07-27 (all HTTP 200). Entirely anonymous - no\n    Authorization header, no API key, no required cookie; the server sets\n    EPiStateMarker and Azure ARRAffinity cookies but does not enforce them.\n    Deliberately NOT listed in apis.yml apis[]: unpublished, unsupported, and\n    covered by no terms of programmatic\
  \ use.\n- name: ERO Portal\n  host: https://eroportal.nerc.net\n  auth: interactive-login\n  scheme: username/password with security questions and a BotDetect CAPTCHA\n    (/BotDetectCaptcha.ashx observed)\n  standards: []\n  note: >-\n    Adxstudio/Dynamics-era customer portal. Account registration, then a separate\n    access request per data store or application, approved by NERC. No OAuth2, no\n    OIDC discovery document (probed paths return the portal's soft-404 HTML error\n    page, not JSON), no client credentials, no machine-to-machine path.\n- name: E-ISAC portal (Salesforce Experience Cloud)\n  host: https://www.eisac.com\n  auth: oauth2 + openIdConnect\n  discovery: https://www.eisac.com/.well-known/openid-configuration\n  discovery_status: 200\n  captured: well-known/nerc-eisac-openid-configuration.json\n  issuer: https://www.eisac.com\n  endpoints:\n    authorization: https://www.eisac.com/services/oauth2/authorize\n    token: https://www.eisac.com/services/oauth2/token\n\
  \    userinfo: https://www.eisac.com/services/oauth2/userinfo\n    introspection: https://www.eisac.com/services/oauth2/introspect\n    revocation: https://www.eisac.com/services/oauth2/revoke\n    registration: https://www.eisac.com/services/oauth2/register\n    end_session: https://www.eisac.com/services/auth/idp/oidc/logout\n    jwks: https://www.eisac.com/id/keys\n  response_types_supported:\n  - code\n  - token\n  - token id_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  scopes_supported_count: 36\n  scopes: scopes/nerc-scopes.yml\n  gated: true\n  note: >-\n    Real, anonymous, standards-compliant OIDC discovery - but it is Salesforce\n    Experience Cloud's stock issuer metadata, not a NERC-authored developer\n    contract. No NERC documentation references it, there is no client-registration\n    path for outside developers,\
  \ and every protected resource behind it is\n    membership-gated: https://www.eisac.com/services/data/v62.0 returns HTTP 401\n    INVALID_SESSION_ID. The anonymous Salesforce version list at /services/data\n    returns HTTP 200. E-ISAC membership is a separate organizational eligibility\n    process, not a developer signup.\n- name: Support desk\n  host: https://support.nerc.net\n  auth: sso\n  scheme: EasyVista SSO (hubzone-prod-us-east.easyvista.com IdP)\n  note: >-\n    Unauthenticated request returns HTTP 503 with \"No active session. Please\n    start a new authentication flow.\" Industry support desk, not developer\n    support.\nnot_found:\n- API keys or developer credentials of any kind\n- Client-credentials / machine-to-machine grant published for any NERC system\n- mTLS or client certificates\n- OIDC discovery on www.nerc.com (/.well-known/openid-configuration -> HTTP 404)\n- Accreditation scheme for programmatic data recipients\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nerc/refs/heads/main/authentication/nerc-authentication.yml
summary_line: none/oauth2/openIdConnect · 0 schemes
tags:
- Energy
- United States
- Canada
- Electricity
- Grid
- Regulator
- Government
- Reliability
- Bulk Power System
- Critical Infrastructure
- Cyber Security
- Energy Markets
- Compliance
---
