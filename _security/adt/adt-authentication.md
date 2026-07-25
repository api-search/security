---
api_key_in: []
api_specs:
- filename: adt-access-codes-api-openapi.yml
  format: yaml
  label: ADT Access Codes API
  slug: adt-access-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-access-codes-api-openapi.yml
- filename: adt-access-control-api-openapi.yml
  format: yaml
  label: ADT Access Control API
  slug: adt-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-access-control-api-openapi.yml
- filename: adt-automation-api-openapi.yml
  format: yaml
  label: ADT Automation API
  slug: adt-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-automation-api-openapi.yml
- filename: adt-devices-api-openapi.yml
  format: yaml
  label: ADT Devices API
  slug: adt-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-devices-api-openapi.yml
- filename: adt-events-api-openapi.yml
  format: yaml
  label: ADT Events API
  slug: adt-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-events-api-openapi.yml
- filename: adt-reports-api-openapi.yml
  format: yaml
  label: ADT Reports API
  slug: adt-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-reports-api-openapi.yml
- filename: adt-security-systems-api-openapi.yml
  format: yaml
  label: ADT Security Systems API
  slug: adt-security-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-security-systems-api-openapi.yml
- filename: adt-sites-api-openapi.yml
  format: yaml
  label: ADT Sites API
  slug: adt-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-sites-api-openapi.yml
- filename: adt-users-api-openapi.yml
  format: yaml
  label: ADT Users API
  slug: adt-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-users-api-openapi.yml
- filename: adt-video-api-openapi.yml
  format: yaml
  label: ADT Video API
  slug: adt-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-video-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Adt Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: ADT secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: ADT
provider_slug: adt
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://auth.adt.com/oauth/token
  name: oauth2
  sources:
  - openapi/adt-business-api-openapi.yml
  type: oauth2
- flows:
  - authorizationUrl: https://auth.adt.com/oauth/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://auth.adt.com/oauth/token
  name: oauth2
  sources:
  - openapi/adt-platform-api-openapi.yml
  type: oauth2
slug: adt-authentication
source_filename: adt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adt-business-api-openapi.yml, openapi/adt-platform-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.adt.com/oauth/token\n    scopes: 4\n  sources:\n  - openapi/adt-business-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.adt.com/oauth/authorize\n    tokenUrl: https://auth.adt.com/oauth/token\n    scopes: 6\n  sources:\n  - openapi/adt-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/authentication/adt-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
- Fortune 1000
---
