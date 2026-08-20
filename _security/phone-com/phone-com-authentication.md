---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Phone Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phone Com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Phone Com
provider_slug: phone-com
scheme_count: 1
schemes:
- bearer_format: opaque
  description: OAuth 2.0 Authorization Framework. Every Phone.com API request requires a valid access token.
  grant_types:
  - authorization_code
  - client_credentials
  - password
  - refresh_token
  header: Authorization
  in: header
  name: oauth2
  scheme_prefix: Bearer
  scopes:
  - account-owner
  - extension-user
  - oauth-management
  - methods:ALL
  token_endpoint: https://api.phone.com/v4/oauth/access-token
  token_endpoint_path: /v4/oauth/access-token
  type: oauth2
slug: phone-com-authentication
source_filename: phone-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://apidocs.phone.com/docs/access-token\ntype: Authentication\napi: phone-com-api\ndocs: https://docs.phone.com/aboutdevenv/insidephonecomapi/apisecurity.html\nsummary: >-\n  The Phone.com v4 API authenticates with OAuth 2.0. Callers present a Bearer\n  access token in the Authorization header (prefixed with the keyword \"Bearer\").\n  All Phone.com API requests require an access token.\nschemes:\n- name: oauth2\n  type: oauth2\n  description: OAuth 2.0 Authorization Framework. Every Phone.com API request requires a valid access token.\n  bearer_format: opaque\n  token_endpoint: https://api.phone.com/v4/oauth/access-token\n  token_endpoint_path: /v4/oauth/access-token\n  in: header\n  header: Authorization\n  scheme_prefix: Bearer\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - password\n  - refresh_token\n  scopes:\n  - account-owner\n  - extension-user\n  - oauth-management\n  - methods:ALL\nnotes:\
  \ >-\n  Scopes are space-separated and may be combined. account-owner and\n  extension-user set the identity/permission tier; oauth-management is required\n  for token- and API-usage-management endpoints; methods:ALL grants access to\n  all API methods. Derived-script path (derive-authentication.py) was not run\n  because no machine-readable OpenAPI is published (the spec sits behind the\n  authenticated api.phone.com host); this profile is transcribed from the\n  published auth docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phone-com/refs/heads/main/authentication/phone-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- VoIP
- Telephony
- Business Phone
- SMS
- Video Conferencing
- Communications
---
