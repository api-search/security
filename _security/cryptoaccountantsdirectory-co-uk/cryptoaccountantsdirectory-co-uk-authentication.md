---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cryptoaccountantsdirectory-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Crypto Accountants Directory Enquiry API
  slug: cryptoaccountantsdirectory-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptoaccountantsdirectory-co-uk/openapi/cryptoaccountantsdirectory-co-uk-enquiry-api-openapi.yml
- filename: cryptoaccountantsdirectory-co-uk-guide-api-openapi.yml
  format: yaml
  label: Crypto Accountants Directory Guide API
  slug: cryptoaccountantsdirectory-co-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptoaccountantsdirectory-co-uk/openapi/cryptoaccountantsdirectory-co-uk-guide-api-openapi.yml
- filename: cryptoaccountantsdirectory-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Crypto Accountants Directory MCP API
  slug: cryptoaccountantsdirectory-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptoaccountantsdirectory-co-uk/openapi/cryptoaccountantsdirectory-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Crypto Accountants Directory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crypto Accountants Directory secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Crypto Accountants Directory
provider_slug: cryptoaccountantsdirectory-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cryptoaccountantsdirectory-co-uk-openapi.json
  type: http
slug: cryptoaccountantsdirectory-co-uk-authentication
source_filename: cryptoaccountantsdirectory-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cryptoaccountantsdirectory-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/cryptoaccountantsdirectory-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cryptoaccountantsdirectory-co-uk/authentication/cryptoaccountantsdirectory-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cryptocurrency
- Accounting
- United Kingdom
- Tax
---
