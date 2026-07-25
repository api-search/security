---
api_key_in: []
api_specs:
- filename: cfpb-aggregations-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Aggregations API
  slug: cfpb-aggregations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-aggregations-api-openapi.yml
- filename: cfpb-complaints-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Complaints API
  slug: cfpb-complaints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-complaints-api-openapi.yml
- filename: cfpb-csv-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) CSV API
  slug: cfpb-csv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-csv-api-openapi.yml
- filename: cfpb-edits-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Edits API
  slug: cfpb-edits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-edits-api-openapi.yml
- filename: cfpb-filers-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Filers API
  slug: cfpb-filers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-filers-api-openapi.yml
- filename: cfpb-filings-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Filings API
  slug: cfpb-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-filings-api-openapi.yml
- filename: cfpb-health-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Health API
  slug: cfpb-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-health-api-openapi.yml
- filename: cfpb-institutions-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Institutions API
  slug: cfpb-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-institutions-api-openapi.yml
- filename: cfpb-submissions-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Submissions API
  slug: cfpb-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-submissions-api-openapi.yml
- filename: cfpb-trends-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Trends API
  slug: cfpb-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-trends-api-openapi.yml
- filename: cfpb-typeahead-api-openapi.yml
  format: yaml
  label: Consumer Financial Protection Bureau (CFPB) Typeahead API
  slug: cfpb-typeahead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/openapi/cfpb-typeahead-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cfpb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Consumer Financial Protection Bureau (CFPB) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Consumer Financial Protection Bureau (CFPB)
provider_slug: cfpb
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cfpb-hmda-filing-api-openapi.yml
  type: http
slug: cfpb-authentication
source_filename: cfpb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cfpb-hmda-filing-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/cfpb-hmda-filing-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cfpb/refs/heads/main/authentication/cfpb-authentication.yml
summary_line: http · 1 scheme
tags:
- Consumer Finance
- Government
- Complaints
- Mortgage
- HMDA
- Financial Data
- Regulatory
- Open Data
---
