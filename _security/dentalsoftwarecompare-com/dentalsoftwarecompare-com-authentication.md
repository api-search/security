---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dentalsoftwarecompare-com-enquiry-api-openapi.yml
  format: yaml
  label: Dental Software Compare Enquiry API
  slug: dentalsoftwarecompare-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dentalsoftwarecompare-com/openapi/dentalsoftwarecompare-com-enquiry-api-openapi.yml
- filename: dentalsoftwarecompare-com-guide-api-openapi.yml
  format: yaml
  label: Dental Software Compare Guide API
  slug: dentalsoftwarecompare-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dentalsoftwarecompare-com/openapi/dentalsoftwarecompare-com-guide-api-openapi.yml
- filename: dentalsoftwarecompare-com-mcp-api-openapi.yml
  format: yaml
  label: Dental Software Compare MCP API
  slug: dentalsoftwarecompare-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dentalsoftwarecompare-com/openapi/dentalsoftwarecompare-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dentalsoftwarecompare Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dental Software Compare secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dental Software Compare
provider_slug: dentalsoftwarecompare-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  optional: true
  scheme: bearer
  sources:
  - openapi/dentalsoftwarecompare-com-openapi.yml
  - https://dentalsoftwarecompare.com/openapi.json
  type: http
slug: dentalsoftwarecompare-com-authentication
source_filename: dentalsoftwarecompare-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://dentalsoftwarecompare.com/openapi.json\ndocs: https://dentalsoftwarecompare.com/mcp\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  optional: true\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/dentalsoftwarecompare-com-openapi.yml\n  - https://dentalsoftwarecompare.com/openapi.json\nnote: 'The MCP server card served at GET https://dentalsoftwarecompare.com/mcp (HTTP 200, 2026-11-05) declares\n  \"auth\": \"none\" for the Streamable HTTP endpoint. Anonymous calls are accepted on a free tier; the bearer\n  access key is optional and raises the caller''s budget. No page documents how to obtain an emk_ key.'\n"
source_yaml_url: https://artifacts.apis.io/dentalsoftwarecompare-com/authentication/dentalsoftwarecompare-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Dental Software
- Practice Management
- Healthcare
- NHS
- Software Comparison
- United Kingdom
- Datasets
---
