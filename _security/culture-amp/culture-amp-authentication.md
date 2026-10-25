---
anonymous_access: false
api_key_in: []
api_specs:
- filename: culture-amp-employees-api-openapi.yml
  format: yaml
  label: Culture Amp Employees API
  slug: culture-amp-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/openapi/culture-amp-employees-api-openapi.yml
- filename: culture-amp-performance-api-openapi.yml
  format: yaml
  label: Culture Amp Performance API
  slug: culture-amp-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/openapi/culture-amp-performance-api-openapi.yml
- filename: culture-amp-surveys-api-openapi.yml
  format: yaml
  label: Culture Amp Surveys API
  slug: culture-amp-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/openapi/culture-amp-surveys-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Culture Amp Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Culture Amp secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Culture Amp
provider_slug: culture-amp
scheme_count: 1
schemes:
- client_auth:
  - client_id/client_secret in form body
  - HTTP Basic (base64 client id:secret)
  flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://api.cultureamp.com/v1/oauth2/token
  name: Oauth2
  scope_format: target-entity:<entity id>:<comma separated list of permissions>
  sources:
  - openapi/culture-amp-employees-api-openapi.yml
  - openapi/culture-amp-performance-api-openapi.yml
  - openapi/culture-amp-surveys-api-openapi.yml
  token:
    expires_in_example: 3599
    format: JWT
    lifetime: Access tokens are valid for 1 hour.
    usage: 'Authorization: Bearer <access token>'
  token_request_content_type: application/x-www-form-urlencoded
  type: oauth2
slug: culture-amp-authentication
source_filename: culture-amp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: searched\nsource:\n- https://docs.api.cultureamp.com/docs/customer-guide-authentication\n- https://docs.api.cultureamp.com/docs/customer-guide-getting-credentials\n- https://docs.api.cultureamp.com/docs/partner-guide-authentication\n- https://docs.api.cultureamp.com/docs/resources-security-information\ndocs: https://docs.api.cultureamp.com/docs/customer-guide-authentication\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.cultureamp.com/v1/oauth2/token\n    scopes: 4\n  client_auth:\n  - client_id/client_secret in form body\n  - HTTP Basic (base64 client id:secret)\n  token_request_content_type: application/x-www-form-urlencoded\n  token:\n    format: JWT\n    usage: 'Authorization: Bearer <access token>'\n    lifetime: Access tokens are valid for 1 hour.\n    expires_in_example: 3599\n  scope_format: target-entity:<entity\
  \ id>:<comma separated list of permissions>\n  sources:\n  - openapi/culture-amp-employees-api-openapi.yml\n  - openapi/culture-amp-performance-api-openapi.yml\n  - openapi/culture-amp-surveys-api-openapi.yml\ncredentials: Created in Admin Settings > API by an Admin user with Account Owner permissions; account-level credentials.\nip_allowlisting: We do not support IP whitelisting.\ntls: Minimum TLS 1.2\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culture-amp/refs/heads/main/authentication/culture-amp-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Human Resources
- Employee Engagement
- Performance Management
- People Analytics
- Surveys
- Australia
---
