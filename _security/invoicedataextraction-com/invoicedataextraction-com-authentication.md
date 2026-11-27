---
anonymous_access: false
api_key_in: []
api_specs:
- filename: invoicedataextraction-com-credits-api-openapi.yml
  format: yaml
  label: Invoice Data Extraction Credits API
  slug: invoicedataextraction-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invoicedataextraction-com/openapi/invoicedataextraction-com-credits-api-openapi.yml
- filename: invoicedataextraction-com-extractions-api-openapi.yml
  format: yaml
  label: Invoice Data Extraction Extractions API
  slug: invoicedataextraction-com-extractions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invoicedataextraction-com/openapi/invoicedataextraction-com-extractions-api-openapi.yml
- filename: invoicedataextraction-com-uploads-api-openapi.yml
  format: yaml
  label: Invoice Data Extraction Uploads API
  slug: invoicedataextraction-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invoicedataextraction-com/openapi/invoicedataextraction-com-uploads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Invoice Data Extraction Authentication
name_suffix: Authentication
oauth_flows: []
overview: Invoice Data Extraction secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Invoice Data Extraction
provider_slug: invoicedataextraction-com
scheme_count: 1
schemes:
- description: 'An API key created at https://invoicedataextraction.com/dashboard?view=API, sent as `Authorization: Bearer YOUR_API_KEY`. Every account includes 50 free pages a month. A team admin''s key sees the team''s extractions by default (the `scope` parameter).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/invoicedataextraction-com-openapi.json
  type: http
slug: invoicedataextraction-com-authentication
source_filename: invoicedataextraction-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/invoicedataextraction-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'An API key created at https://invoicedataextraction.com/dashboard?view=API,\n    sent as `Authorization: Bearer YOUR_API_KEY`. Every account includes 50 free pages a month.\n    A team admin''s key sees the team''s extractions by default (the `scope` parameter).'\n  sources:\n  - openapi/invoicedataextraction-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/invoicedataextraction-com/authentication/invoicedataextraction-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Artificial Intelligence
- Data Extraction
- Invoicing
- Automation
---
