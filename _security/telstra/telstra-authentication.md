---
api_key_in: []
api_specs:
- filename: telstra-messaging-api-openapi.yml
  format: yaml
  label: Telstra Messaging API
  slug: telstra-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telstra/refs/heads/main/openapi/telstra-messaging-api-openapi.yml
- filename: telstra-mobile-number-verification-api-openapi.yml
  format: yaml
  label: Telstra Mobile Number Verification API
  slug: telstra-mobile-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telstra/refs/heads/main/openapi/telstra-mobile-number-verification-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Telstra Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Telstra secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Telstra
provider_slug: telstra
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials grant against https://tapi.telstra.com/v2/oauth/token with the NSMS scope.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://tapi.telstra.com/v2/oauth/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/telstra-messaging-api-openapi.yml
  - openapi/telstra-mobile-number-verification-api-openapi.yml
  type: oauth2
slug: telstra-authentication
source_filename: telstra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telstra-messaging-api-openapi.yml, openapi/telstra-mobile-number-verification-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://tapi.telstra.com/v2/oauth/token\n    scopes: 1\n  description: OAuth 2.0 client credentials grant against https://tapi.telstra.com/v2/oauth/token\n    with the NSMS scope.\n  sources:\n  - openapi/telstra-messaging-api-openapi.yml\n  - openapi/telstra-mobile-number-verification-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telstra/refs/heads/main/authentication/telstra-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Telecommunications
- Telco
- Mobile
- Messaging
- SMS
- MMS
- Networks
- Australia
- Verification
---
