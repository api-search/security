---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cqcregistrationchecker-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: CQC Registration Checker Enquiry API
  slug: cqcregistrationchecker-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqcregistrationchecker-co-uk/openapi/cqcregistrationchecker-co-uk-enquiry-api-openapi.yml
- filename: cqcregistrationchecker-co-uk-guide-api-openapi.yml
  format: yaml
  label: CQC Registration Checker Guide API
  slug: cqcregistrationchecker-co-uk-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqcregistrationchecker-co-uk/openapi/cqcregistrationchecker-co-uk-guide-api-openapi.yml
- filename: cqcregistrationchecker-co-uk-mcp-api-openapi.yml
  format: yaml
  label: CQC Registration Checker MCP API
  slug: cqcregistrationchecker-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cqcregistrationchecker-co-uk/openapi/cqcregistrationchecker-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: CQC Registration Checker Authentication
name_suffix: Authentication
oauth_flows: []
overview: CQC Registration Checker secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CQC Registration Checker
provider_slug: cqcregistrationchecker-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/cqcregistrationchecker-co-uk-openapi.yml
  type: http
slug: cqcregistrationchecker-co-uk-authentication
source_filename: cqcregistrationchecker-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/cqcregistrationchecker-co-uk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity\n    export requires one.'\n  sources:\n  - openapi/cqcregistrationchecker-co-uk-openapi.yml\noptional: true\nanonymous_access: 'The spec marks every tool operation with security [{}, {accessKey: []}] - unauthenticated\n  calls are allowed on a free tier; a bearer access key (emk_...) raises the ceiling.'\nmcp_card_auth: none\ndocs: https://cqcregistrationchecker.co.uk/mcp\nnote: The MCP server card at https://cqcregistrationchecker.co.uk/mcp (GET 200, 2026-11-04) declares \"auth\":\"none\"\n  for the streamable-http MCP endpoint. The 429 response text points to \"docs/MCP.md\" for access keys,\n  but https://cqcregistrationchecker.co.uk/docs/MCP.md returned 404 on 2026-11-04; no public\
  \ page documents\n  how to obtain an emk_ key.\n"
source_yaml_url: https://artifacts.apis.io/cqcregistrationchecker-co-uk/authentication/cqcregistrationchecker-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Care Quality Commission
- Regulatory Compliance
- Social Care
- United Kingdom
- Datasets
---
