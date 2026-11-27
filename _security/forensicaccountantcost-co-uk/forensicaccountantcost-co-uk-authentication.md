---
anonymous_access: false
api_key_in: []
api_specs:
- filename: forensicaccountantcost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Forensic Accountant Cost Enquiry API
  slug: forensicaccountantcost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forensicaccountantcost-co-uk/openapi/forensicaccountantcost-co-uk-enquiry-api-openapi.yml
- filename: forensicaccountantcost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Forensic Accountant Cost MCP API
  slug: forensicaccountantcost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forensicaccountantcost-co-uk/openapi/forensicaccountantcost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Forensic Accountant Cost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forensic Accountant Cost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Forensic Accountant Cost
provider_slug: forensicaccountantcost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/forensicaccountantcost-co-uk-openapi.yml
  type: http
slug: forensicaccountantcost-co-uk-authentication
source_filename: forensicaccountantcost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/forensicaccountantcost-co-uk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/forensicaccountantcost-co-uk-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/forensicaccountantcost-co-uk/authentication/forensicaccountantcost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Forensics
- Accounting
- United Kingdom
- Legal
- Pricing
---
