---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Datafy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datafy declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Datafy
provider_slug: datafy
scheme_count: 1
schemes:
- applies_to: all endpoints
  description: A user-specific bearer token generated from the API Access page inside the Datafy portal. Datafy's docs state the value has the format "<Bearer token-string>" and that "the entire string including 'Bearer' is required" — i.e. the caller sends the full "Bearer <token>" value in the Authorization header.
  header: Authorization
  in: header
  key: bearerToken
  required: true
  scheme: bearer
  source: https://www.datafy.com/docs
  type: http
slug: datafy-authentication
source_filename: datafy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://www.datafy.com/docs\ndocs: https://www.datafy.com/docs\nnote: >-\n  Datafy publishes no OpenAPI, so this profile is read from the provider's own\n  public API documentation (\"Requesting an API Token\" section) and confirmed\n  against the live behaviour of https://api.datafy.com/, which answers every\n  anonymous request with a JSON UnauthorizedError.\napi: Datafy Data API\nbase_url: https://api.datafy.com/\nschemes:\n- key: bearerToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: >-\n    A user-specific bearer token generated from the API Access page inside the\n    Datafy portal. Datafy's docs state the value has the format\n    \"<Bearer token-string>\" and that \"the entire string including 'Bearer' is\n    required\" — i.e. the caller sends the full \"Bearer <token>\" value in the\n    Authorization header.\n  required: true\n  applies_to: all endpoints\n  source: https://www.datafy.com/docs\n\
  oauth2: false\nopenid_connect: false\nmutual_tls: false\napi_key_query_param: false\nscopes:\n  model: none\n  note: >-\n    No OAuth scopes and no permission strings are documented. Authorization is\n    coarse — a token carries the destinations and levels that user's account is\n    entitled to, and the /options endpoint is how a caller discovers what its own\n    token is allowed to request.\ntoken_issuance:\n  self_service: false\n  where: https://portal.datafy.com\n  page: API Access page (inside the portal, after sign-in)\n  prerequisite: >-\n    \"Reach out to your CX representative to gain visibility to our API Access\n    Page.\" The API Access page is not visible to a portal user until Datafy's\n    customer-experience team enables it, so token issuance is gated on a human\n    at Datafy, not on self-service signup.\n  scope_of_token: user-specific; Datafy states tokens must not be shared and that\n    unauthorized sharing may result in access being revoked\ntoken_lifecycle:\n\
  \  expires: true\n  lifetime_days: 30\n  rotation: manual\n  renewal_window_days: 6\n  renewal_note: >-\n    \"Tokens will expire every 30 days and a refreshed token can be requested at\n    the api access page within 6 days of the prior token's expiration.\" There is\n    no refresh-token grant and no programmatic rotation endpoint — renewal is a\n    human action in the portal, which means any unattended agent integration will\n    break on a 30-day cycle unless a person rotates the credential.\n  revocation: >-\n    Datafy states it may revoke access for token sharing; no self-service\n    revocation endpoint or page is documented.\nobserved_unauthenticated_behaviour:\n  probed: '2026-08-12'\n  request: GET https://api.datafy.com/ with no Authorization header\n  http_status: 500\n  content_type: application/json; charset=utf-8\n  body_shape: '{\"name\":\"UnauthorizedError\",\"message\":\"No authorization token was found\",\"stack\":\"...\"}'\n  finding: >-\n    The API returns HTTP\
  \ 500 rather than 401 for a missing credential, and the\n    JSON body includes a server-side stack trace with internal file paths. Both\n    are defects a caller has to code around: an agent cannot distinguish \"you are\n    not authenticated\" from \"the service is broken\" by status code alone, and\n    there is no WWW-Authenticate challenge to discover the scheme from.\ngaps:\n- No machine-readable securityScheme is published (no OpenAPI, no\n  /.well-known/openid-configuration, no /.well-known/oauth-protected-resource).\n- Missing credential returns 500, not 401, and emits a stack trace.\n- No programmatic token refresh; 30-day manual rotation in a portal.\n- Token issuance requires a customer-experience representative to unlock the API\n  Access page, so the credential path is not self-service.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datafy/refs/heads/main/authentication/datafy-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Analytics
- Advertising
- Location Intelligence
- Attribution
- Tourism
- Marketing
- Visitation Data
- Destination Marketing
- Measurement
---
