---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hemrock-com-access-api-openapi.yml
  format: yaml
  label: Hemrock Access API
  slug: hemrock-com-access-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-access-api-openapi.yml
- filename: hemrock-com-cap-table-api-openapi.yml
  format: yaml
  label: Hemrock Cap Table API
  slug: hemrock-com-cap-table-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-cap-table-api-openapi.yml
- filename: hemrock-com-compute-api-openapi.yml
  format: yaml
  label: Hemrock Compute API
  slug: hemrock-com-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-compute-api-openapi.yml
- filename: hemrock-com-ecommerce-forecasting-api-openapi.yml
  format: yaml
  label: Hemrock Ecommerce Forecasting API
  slug: hemrock-com-ecommerce-forecasting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-ecommerce-forecasting-api-openapi.yml
- filename: hemrock-com-exit-waterfall-api-openapi.yml
  format: yaml
  label: Hemrock Exit Waterfall API
  slug: hemrock-com-exit-waterfall-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-exit-waterfall-api-openapi.yml
- filename: hemrock-com-fund-economics-api-openapi.yml
  format: yaml
  label: Hemrock Fund Economics API
  slug: hemrock-com-fund-economics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-fund-economics-api-openapi.yml
- filename: hemrock-com-models-api-openapi.yml
  format: yaml
  label: Hemrock Models API
  slug: hemrock-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-models-api-openapi.yml
- filename: hemrock-com-results-api-openapi.yml
  format: yaml
  label: Hemrock Results API
  slug: hemrock-com-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-results-api-openapi.yml
- filename: hemrock-com-saas-forecasting-api-openapi.yml
  format: yaml
  label: Hemrock Saas Forecasting API
  slug: hemrock-com-saas-forecasting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-saas-forecasting-api-openapi.yml
- filename: hemrock-com-unit-economics-api-openapi.yml
  format: yaml
  label: Hemrock Unit Economics API
  slug: hemrock-com-unit-economics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-unit-economics-api-openapi.yml
- filename: hemrock-com-usage-api-openapi.yml
  format: yaml
  label: Hemrock Usage API
  slug: hemrock-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hemrock-com/openapi/hemrock-com-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hemrock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hemrock secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hemrock
provider_slug: hemrock-com
scheme_count: 1
schemes:
- description: 'Your API key (`hk_live_…`), created in the Hemrock developer dashboard. Calls use that account’s product access: lifetime free credits or an active paid allowance.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hemrock-com-openapi.json
  - openapi/hemrock_com_openapi.json
  type: http
slug: hemrock-com-authentication
source_filename: hemrock-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hemrock-com-openapi.json, openapi/hemrock_com_openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Your API key (`hk_live_…`), created in the Hemrock developer dashboard. Calls\n    use that account’s product access: lifetime free credits or an active paid allowance.'\n  sources:\n  - openapi/hemrock-com-openapi.json\n  - openapi/hemrock_com_openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hemrock-com/authentication/hemrock-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Open Source
- Artificial Intelligence
- Modeling
- Community
- Company
---
