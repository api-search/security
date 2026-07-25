---
api_key_in:
- query
api_specs:
- filename: doe-aeo-api-openapi.yml
  format: yaml
  label: Department of Energy AEO API
  slug: doe-aeo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-aeo-api-openapi.yml
- filename: doe-coal-api-openapi.yml
  format: yaml
  label: Department of Energy COAL API
  slug: doe-coal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-coal-api-openapi.yml
- filename: doe-crud-imports-api-openapi.yml
  format: yaml
  label: Department of Energy CRUD_IMPORTS API
  slug: doe-crud-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-crud-imports-api-openapi.yml
- filename: doe-dbf-api-openapi.yml
  format: yaml
  label: Department of Energy DBF API
  slug: doe-dbf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-dbf-api-openapi.yml
- filename: doe-elec-api-openapi.yml
  format: yaml
  label: Department of Energy ELEC API
  slug: doe-elec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-elec-api-openapi.yml
- filename: doe-emiss-api-openapi.yml
  format: yaml
  label: Department of Energy EMISS API
  slug: doe-emiss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-emiss-api-openapi.yml
- filename: doe-ieo-api-openapi.yml
  format: yaml
  label: Department of Energy IEO API
  slug: doe-ieo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-ieo-api-openapi.yml
- filename: doe-intl-api-openapi.yml
  format: yaml
  label: Department of Energy INTL API
  slug: doe-intl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-intl-api-openapi.yml
- filename: doe-ng-api-openapi.yml
  format: yaml
  label: Department of Energy NG API
  slug: doe-ng-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-ng-api-openapi.yml
- filename: doe-nuc-status-api-openapi.yml
  format: yaml
  label: Department of Energy NUC_STATUS API
  slug: doe-nuc-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-nuc-status-api-openapi.yml
- filename: doe-root-api-openapi.yml
  format: yaml
  label: Department of Energy Root API
  slug: doe-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-root-api-openapi.yml
- filename: doe-rto-api-openapi.yml
  format: yaml
  label: Department of Energy RTO API
  slug: doe-rto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-rto-api-openapi.yml
- filename: doe-seds-api-openapi.yml
  format: yaml
  label: Department of Energy SEDS API
  slug: doe-seds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-seds-api-openapi.yml
- filename: doe-sep-api-openapi.yml
  format: yaml
  label: Department of Energy SEP API
  slug: doe-sep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-sep-api-openapi.yml
- filename: doe-steo-api-openapi.yml
  format: yaml
  label: Department of Energy STEO API
  slug: doe-steo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-steo-api-openapi.yml
- filename: doe-total-api-openapi.yml
  format: yaml
  label: Department of Energy TOTAL API
  slug: doe-total-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/openapi/doe-total-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Doe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Department of Energy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Department of Energy
provider_slug: doe
scheme_count: 1
schemes:
- in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/eia-open-data-api-openapi.yaml
  type: apiKey
slug: doe-authentication
source_filename: doe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/eia-open-data-api-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/eia-open-data-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doe/refs/heads/main/authentication/doe-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- Government
- Renewable Energy
- Electricity
- Natural Gas
- Petroleum
- Solar
- Wind
- Electric Vehicles
- Alternative Fuels
- Nuclear
- Scientific Research
---
