---
api_key_in:
- header
api_specs:
- filename: esper-application-api-openapi.yml
  format: yaml
  label: Esper Application API
  slug: esper-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-application-api-openapi.yml
- filename: esper-application-v1-api-openapi.yml
  format: yaml
  label: Esper Application V1 API
  slug: esper-application-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-application-v1-api-openapi.yml
- filename: esper-commands-api-openapi.yml
  format: yaml
  label: Esper Commands API
  slug: esper-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-commands-api-openapi.yml
- filename: esper-commands-v2-api-openapi.yml
  format: yaml
  label: Esper Commands V2 API
  slug: esper-commands-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-commands-v2-api-openapi.yml
- filename: esper-content-api-openapi.yml
  format: yaml
  label: Esper Content API
  slug: esper-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-content-api-openapi.yml
- filename: esper-device-api-openapi.yml
  format: yaml
  label: Esper Device API
  slug: esper-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-device-api-openapi.yml
- filename: esper-device-group-api-openapi.yml
  format: yaml
  label: Esper Device Group API
  slug: esper-device-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-device-group-api-openapi.yml
- filename: esper-enterprise-api-openapi.yml
  format: yaml
  label: Esper Enterprise API
  slug: esper-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-enterprise-api-openapi.yml
- filename: esper-enterprise-policy-api-openapi.yml
  format: yaml
  label: Esper Enterprise Policy API
  slug: esper-enterprise-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-enterprise-policy-api-openapi.yml
- filename: esper-geofence-api-openapi.yml
  format: yaml
  label: Esper Geofence API
  slug: esper-geofence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-geofence-api-openapi.yml
- filename: esper-group-commands-api-openapi.yml
  format: yaml
  label: Esper Group Commands API
  slug: esper-group-commands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-group-commands-api-openapi.yml
- filename: esper-subscription-api-openapi.yml
  format: yaml
  label: Esper Subscription API
  slug: esper-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-subscription-api-openapi.yml
- filename: esper-token-api-openapi.yml
  format: yaml
  label: Esper Token API
  slug: esper-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/openapi/esper-token-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Esper Authentication
name_suffix: Authentication
oauth_flows: []
overview: Esper secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Esper
provider_slug: esper
scheme_count: 1
schemes:
- description: '#### API KEY - Access Token

    Access token for APIs passed as authorization header in calls. You need to generate this from your Esper Dev Console at `<domain>-api.esper.cloud` where foo is the sub-domain name you gave for your Esper Dev environment when you signed up for your Esper Dev account. Please follow the instructions [here](https://docs.esper.io/home/module/genapikey.html) to generate an ac'
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/esper-manage-openapi-original.yml
  type: apiKey
slug: esper-authentication
source_filename: esper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/esper-manage-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    #### API KEY - Access Token\n    Access token for APIs passed as authorization header in calls. You need to generate this from your Esper Dev Console at `<domain>-api.esper.cloud` where foo is the sub-domain name you gave for your Esper Dev environment when you signed up for your Esper Dev account. Please follow the instructions [here](https://docs.esper.io/home/module/genapikey.html) to generate an ac\n  sources:\n  - openapi/esper-manage-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esper/refs/heads/main/authentication/esper-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Device Management
- Mobile Device Management
- Android
- DevOps
- Internet of Things
- Fleet Management
- Enterprise Mobility
- Edge Computing
- Kiosk
---
