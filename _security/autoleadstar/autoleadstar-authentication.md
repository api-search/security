---
api_key_in: []
api_specs:
- filename: autoleadstar-activities-api-openapi.yml
  format: yaml
  label: AutoLeadStar Activities API
  slug: autoleadstar-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-activities-api-openapi.yml
- filename: autoleadstar-appointments-api-openapi.yml
  format: yaml
  label: AutoLeadStar Appointments API
  slug: autoleadstar-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-appointments-api-openapi.yml
- filename: autoleadstar-audiences-api-openapi.yml
  format: yaml
  label: AutoLeadStar Audiences API
  slug: autoleadstar-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-audiences-api-openapi.yml
- filename: autoleadstar-consents-api-openapi.yml
  format: yaml
  label: AutoLeadStar Consents API
  slug: autoleadstar-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-consents-api-openapi.yml
- filename: autoleadstar-leads-api-openapi.yml
  format: yaml
  label: AutoLeadStar Leads API
  slug: autoleadstar-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-leads-api-openapi.yml
- filename: autoleadstar-shoppers-api-openapi.yml
  format: yaml
  label: AutoLeadStar Shoppers API
  slug: autoleadstar-shoppers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-shoppers-api-openapi.yml
- filename: autoleadstar-tasks-api-openapi.yml
  format: yaml
  label: AutoLeadStar Tasks API
  slug: autoleadstar-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-tasks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Autoleadstar Authentication
name_suffix: Authentication
oauth_flows: []
overview: AutoLeadStar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AutoLeadStar
provider_slug: autoleadstar
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Platform JWT or Consent Management vendor API key.

    In Scalar, paste only the raw token/key (no `Bearer ` prefix).'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/autoleadstar-fullpath-api-openapi.yml
  type: http
slug: autoleadstar-authentication
source_filename: autoleadstar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: openapi/autoleadstar-fullpath-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Platform JWT or Consent Management vendor API key.\n    In Scalar, paste only the raw token/key (no `Bearer ` prefix).\n  sources:\n  - openapi/autoleadstar-fullpath-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/authentication/autoleadstar-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Automotive
- Customer Data Platform
- Marketing Automation
- Dealerships
- Advertising
- Artificial Intelligence
- Consent Management
- CRM
- Israel
---
