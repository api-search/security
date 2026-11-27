---
anonymous_access: true
api_key_in: []
api_specs:
- filename: contractorleadquotes-com-dataset-api-openapi.yml
  format: yaml
  label: Contractor Lead Quotes Dataset API
  slug: contractorleadquotes-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contractorleadquotes-com/openapi/contractorleadquotes-com-dataset-api-openapi.yml
- filename: contractorleadquotes-com-enquiry-api-openapi.yml
  format: yaml
  label: Contractor Lead Quotes Enquiry API
  slug: contractorleadquotes-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contractorleadquotes-com/openapi/contractorleadquotes-com-enquiry-api-openapi.yml
- filename: contractorleadquotes-com-mcp-api-openapi.yml
  format: yaml
  label: Contractor Lead Quotes MCP API
  slug: contractorleadquotes-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contractorleadquotes-com/openapi/contractorleadquotes-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Contractor Lead Quotes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contractor Lead Quotes secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Contractor Lead Quotes
provider_slug: contractorleadquotes-com
scheme_count: 2
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  key_prefix: emk_
  name: accessKey
  scheme: bearer
  sources:
  - openapi/contractorleadquotes-com-openapi.yml
  - https://contractorleadquotes.com/openapi.json
  type: http
- description: The MCP card at https://contractorleadquotes.com/mcp declares "auth":"none", "stateless":true for transport streamable-http (protocolVersions 2025-06-18, 2025-03-26).
  name: none
  sources:
  - https://contractorleadquotes.com/mcp
  type: none
slug: contractorleadquotes-com-authentication
source_filename: contractorleadquotes-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://contractorleadquotes.com/mcp\ndocs: https://contractorleadquotes.com/mcp\nsummary:\n  types:\n  - http\n  optional: true\n  note: 'Every operation in the provider''s OpenAPI declares security [{}, {accessKey: []}] -- anonymous calls are\n    allowed (free tier) and a bearer access key is optional. The provider''s MCP card (GET /mcp) states\n    \"auth\":\"none\" for the Streamable HTTP endpoint.'\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  key_prefix: emk_\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/contractorleadquotes-com-openapi.yml\n  - https://contractorleadquotes.com/openapi.json\n- name: none\n  type: none\n  description: 'The MCP card at https://contractorleadquotes.com/mcp declares \"auth\":\"none\", \"stateless\":true for\n    transport streamable-http (protocolVersions 2025-06-18,\
  \ 2025-03-26).'\n  sources:\n  - https://contractorleadquotes.com/mcp\nissuance:\n  note: The docs do not say how an emk_ access key is obtained. The site links a \"Sign in\" page\n    (https://contractorleadquotes.com/account/), which was not called.\n"
source_yaml_url: https://artifacts.apis.io/contractorleadquotes-com/authentication/contractorleadquotes-com-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Contractor Leads
- Lead Generation
- Home Services
- Pricing Data
- Construction
- Datasets
---
