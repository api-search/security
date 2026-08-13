---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Integral Ad Science Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Integral Ad Science declares 0 security scheme(s) across its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Integral Ad Science
provider_slug: integral-ad-science
scheme_count: 0
schemes: []
slug: integral-ad-science-authentication
source_filename: integral-ad-science-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://helpcenter.integralplatform.com/article/reporting-api — Integral Ad\n  Science Help Center, \"Reporting API\", document dated Jul 11, 2024. The live\n  article now returns 404 to anonymous requests (IAS moved its developer\n  articles behind the IAS Signal login in 2025); the version read here is IAS's\n  own published copy preserved at\n  https://web.archive.org/web/20241015182444/https://helpcenter.integralplatform.com/article/reporting-api\ndocs: https://helpcenter.integralplatform.com/article/developers-center\nnote: >-\n  Derived from IAS's own documentation, then confirmed against the live API\n  host. Not derived from an OpenAPI — Integral Ad Science publishes no\n  machine-readable specification for any of its APIs.\nx-evidence:\n  fetched: '2026-08-12'\n  live_probe:\n    url: https://data.integralplatform.com/report\n    method: GET\n    request_header: 'Authorization: Bearer <invalid>'\n    http_status:\
  \ 401\n    response_body: 'invalid_token: Access token expired'\n    conclusion: >-\n      The host is a live OAuth 2.0 bearer-protected resource server and returns\n      the exact error string IAS documents. Without an Authorization header the\n      same path answers 302 to /spa/login.\n  docs_probe:\n    url: https://helpcenter.integralplatform.com/article/developers-center\n    http_status: 200\n    finding: >-\n      Page renders with requiredRoles [\"loggedIn\"]; the anonymous response\n      carries the title and meta description (\"These guides are for a technical\n      audience who want to use the various IAS APIs and, or integrations\") but\n      no article body.\nsecurity_schemes:\n  - key: iasOAuth2Password\n    type: oauth2\n    flow: password\n    description: >-\n      OAuth 2.0 Resource Owner Password Credentials grant (RFC 6749 §4.3). The\n      username and password are the customer's IAS Signal platform credentials.\n      The client_id / client_secret pair is issued\
  \ out-of-band by an IAS\n      representative — there is no self-serve client registration.\n    token_url: https://data.integralplatform.com/auth/uaa/oauth/token\n    authorization_url: null\n    client_authentication: HTTP Basic (client_id:client_secret)\n    grant_parameters:\n      - grant_type=password\n      - username\n      - password\n    token_response_field: access_token\n    scopes: []\n    scopes_documented: false\n  - key: iasBearer\n    type: http\n    scheme: bearer\n    bearer_format: JWT (UAA-issued access token)\n    description: >-\n      The access_token returned by the token endpoint is presented as\n      \"Authorization: Bearer <token>\" on every Reporting API request. IAS\n      documents token reuse across requests until expiry.\n    in: header\n    parameter_name: Authorization\nsummary:\n  auth_types:\n    - oauth2\n    - http-bearer\n  oauth2_flows:\n    - password\n  api_key_locations: []\n  mutual_tls: false\n  openid_connect: false\n  self_serve_credentials:\
  \ false\n  credential_issuance: >-\n    Sales/account-managed. IAS documents \"Coordinate with your IAS\n    representative to obtain a client ID and client secret.\"\ntoken_lifecycle:\n  expiry_signal:\n    error: invalid_token\n    error_description: Access token expired\n    http_status: 401\n  refresh_documented: false\n  revocation_documented: false\n  rotation_documented: false\ngaps:\n  - No /.well-known/oauth-authorization-server or /.well-known/openid-configuration\n    is served on data.integralplatform.com (both probed 404, 2026-08-12), so the\n    authorization server is not machine-discoverable.\n  - No scopes are documented; authorization is enforced per IAS \"team ID\"\n    membership rather than by OAuth scope.\n  - The password grant is deprecated by OAuth 2.0 Security Best Current Practice\n    (RFC 9700) and omitted from OAuth 2.1; IAS documents no alternative flow.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/integral-ad-science/refs/heads/main/authentication/integral-ad-science-authentication.yml
summary_line: 0 schemes
tags:
- Advertising
- Ad Verification
- Ad Measurement
- Brand Safety
- Ad Fraud
- Viewability
- Contextual Targeting
- Attention Measurement
- CTV
- Connected TV
- Video Advertising
- Programmatic
- Header Bidding
- Prebid
- AdTech
- Marketing
- Media Quality
---
