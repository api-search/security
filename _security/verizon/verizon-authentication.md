---
api_key_in: []
api_specs:
- filename: verizon-accounts-api-openapi.yml
  format: yaml
  label: Verizon Accounts API
  slug: verizon-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/openapi/verizon-accounts-api-openapi.yml
- filename: verizon-callbacks-api-openapi.yml
  format: yaml
  label: Verizon Callbacks API
  slug: verizon-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/openapi/verizon-callbacks-api-openapi.yml
- filename: verizon-devices-api-openapi.yml
  format: yaml
  label: Verizon Devices API
  slug: verizon-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/openapi/verizon-devices-api-openapi.yml
- filename: verizon-session-api-openapi.yml
  format: yaml
  label: Verizon Session API
  slug: verizon-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/openapi/verizon-session-api-openapi.yml
- filename: verizon-sms-api-openapi.yml
  format: yaml
  label: Verizon SMS API
  slug: verizon-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/openapi/verizon-sms-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Verizon Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Verizon secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Verizon
provider_slug: verizon
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://thingspace.verizon.com/api/m2m/v2/session/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/verizon-thingspace-connectivity-openapi.yml
  type: oauth2
slug: verizon-authentication
source_filename: verizon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/verizon-thingspace-connectivity-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://thingspace.verizon.com/api/m2m/v2/session/token\n    scopes: 3\n  sources:\n  - openapi/verizon-thingspace-connectivity-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verizon/refs/heads/main/authentication/verizon-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Wireless
- Telecommunications
- IoT
- 5G
- Enterprise
- Network APIs
- Fortune 100
---
