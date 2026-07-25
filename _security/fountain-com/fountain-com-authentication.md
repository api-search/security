---
api_key_in:
- header
api_specs:
- filename: fountain-com-applicants-api-openapi.yml
  format: yaml
  label: Fountain Applicants API
  slug: fountain-com-applicants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-applicants-api-openapi.yml
- filename: fountain-com-documents-api-openapi.yml
  format: yaml
  label: Fountain Documents API
  slug: fountain-com-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-documents-api-openapi.yml
- filename: fountain-com-labels-api-openapi.yml
  format: yaml
  label: Fountain Labels API
  slug: fountain-com-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-labels-api-openapi.yml
- filename: fountain-com-openings-api-openapi.yml
  format: yaml
  label: Fountain Openings API
  slug: fountain-com-openings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-openings-api-openapi.yml
- filename: fountain-com-positions-api-openapi.yml
  format: yaml
  label: Fountain Positions API
  slug: fountain-com-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-positions-api-openapi.yml
- filename: fountain-com-scheduling-api-openapi.yml
  format: yaml
  label: Fountain Scheduling API
  slug: fountain-com-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-scheduling-api-openapi.yml
- filename: fountain-com-stages-api-openapi.yml
  format: yaml
  label: Fountain Stages API
  slug: fountain-com-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-stages-api-openapi.yml
- filename: fountain-com-webhooks-api-openapi.yml
  format: yaml
  label: Fountain Webhooks API
  slug: fountain-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-webhooks-api-openapi.yml
- filename: fountain-com-workers-api-openapi.yml
  format: yaml
  label: Fountain Workers API
  slug: fountain-com-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/openapi/fountain-com-workers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fountain Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fountain secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fountain
provider_slug: fountain-com
scheme_count: 1
schemes:
- description: Your Fountain API token. Request API access by emailing support@fountain.com; find your token in your Fountain account settings.
  in: header
  name: AccessToken
  parameter: X-ACCESS-TOKEN
  sources:
  - openapi/fountain-com-openapi.yml
  type: apiKey
slug: fountain-com-authentication
source_filename: fountain-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fountain-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: X-ACCESS-TOKEN\n  description: Your Fountain API token. Request API access by emailing support@fountain.com;\n    find your token in your Fountain account settings.\n  sources:\n  - openapi/fountain-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fountain-com/refs/heads/main/authentication/fountain-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Hiring
- Recruiting
- Applicant Tracking
- Frontline Hiring
- Hourly Workforce
- HR Tech
- Onboarding
---
