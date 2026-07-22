---
api_key_in: []
api_specs:
- filename: myfitnesspal-notifications-asyncapi.yml
  format: yaml
  label: MyFitnessPal API v2
  slug: myfitnesspal-api-v2
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/myfitnesspal/refs/heads/main/asyncapi/myfitnesspal-notifications-asyncapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Myfitnesspal Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MyFitnessPal secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MyFitnessPal
provider_slug: myfitnesspal
scheme_count: 2
schemes:
- description: OAuth 2.0 authorization-code grant. A partner application redirects the user to the MyFitnessPal authorization endpoint, receives an authorization code on consent, and exchanges it at the token endpoint for an access token and refresh token. Access tokens authorize subsequent /v2/ requests; refresh tokens obtain new access tokens on expiry. Tokens can be revoked.
  flows:
  - authorizationUrl: https://api.myfitnesspal.com/v2/oauth2/auth
    flow: authorizationCode
    revocationUrl: https://api.myfitnesspal.com/v2/oauth2/revoke
    scopes:
    - diary
    - measurements
    - private-exercises
    - subscriptions
    tokenUrl: https://api.myfitnesspal.com/v2/oauth2/token
  name: OAuth2
  sources:
  - https://myfitnesspalapi.com/docs/auth-example-2
  type: oauth2
- contact: partners@myfitnesspal.com
  description: Partners are issued a Client ID (public, identifies the partner application) and a Client Secret (private, must never be transmitted in plaintext). The Client ID is passed on every request in the mfp-client-id HTTP header; the optional mfp-user-id header scopes a request to a specific user.
  name: PartnerCredentials
  type: client
slug: myfitnesspal-authentication
source_filename: myfitnesspal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://myfitnesspalapi.com/docs\ndocs: https://myfitnesspalapi.com/docs/user-authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  client_auth: client_id + client_secret (partner credentials)\n  required_headers: [mfp-client-id]\n  optional_headers: [mfp-user-id]\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization-code grant. A partner application redirects the user to the MyFitnessPal\n    authorization endpoint, receives an authorization code on consent, and exchanges it at the token\n    endpoint for an access token and refresh token. Access tokens authorize subsequent /v2/ requests;\n    refresh tokens obtain new access tokens on expiry. Tokens can be revoked.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.myfitnesspal.com/v2/oauth2/auth\n    tokenUrl: https://api.myfitnesspal.com/v2/oauth2/token\n    revocationUrl: https://api.myfitnesspal.com/v2/oauth2/revoke\n\
  \    scopes:\n    - diary\n    - measurements\n    - private-exercises\n    - subscriptions\n  sources: [https://myfitnesspalapi.com/docs/auth-example-2]\n- name: PartnerCredentials\n  type: client\n  description: >-\n    Partners are issued a Client ID (public, identifies the partner application) and a Client Secret\n    (private, must never be transmitted in plaintext). The Client ID is passed on every request in the\n    mfp-client-id HTTP header; the optional mfp-user-id header scopes a request to a specific user.\n  contact: partners@myfitnesspal.com\nnotes:\n- The developer program is currently closed to new applicants (\"We are not accepting requests for API access at this time.\").\n- No OpenAPI/Swagger specification is published; this profile is derived from the human docs at myfitnesspalapi.com/docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/myfitnesspal/refs/heads/main/authentication/myfitnesspal-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Consumer
- Health and Fitness
- Nutrition
- Fitness Tracking
- Food Diary
- Wellness
- Webhooks
- OAuth
---
