---
anonymous_access: true
api_key_in: []
api_specs:
- filename: comparefairly-com-comparefairly-api-openapi.yml
  format: yaml
  label: CompareFairly Compare Fairly API
  slug: comparefairly-com-comparefairly-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparefairly-com/openapi/comparefairly-com-comparefairly-api-openapi.yml
- filename: comparefairly-com-llms-txt-api-openapi.yml
  format: yaml
  label: CompareFairly Llms.txt API
  slug: comparefairly-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparefairly-com/openapi/comparefairly-com-llms-txt-api-openapi.yml
- filename: comparefairly-com-mcp-api-openapi.yml
  format: yaml
  label: CompareFairly MCP API
  slug: comparefairly-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparefairly-com/openapi/comparefairly-com-mcp-api-openapi.yml
- filename: comparefairly-com-sitemap-comparatifs-xml-api-openapi.yml
  format: yaml
  label: CompareFairly Sitemap Comparatifs.xml API
  slug: comparefairly-com-sitemap-comparatifs-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparefairly-com/openapi/comparefairly-com-sitemap-comparatifs-xml-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: CompareFairly Authentication
name_suffix: Authentication
oauth_flows: []
overview: CompareFairly declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: CompareFairly
provider_slug: comparefairly-com
scheme_count: 1
schemes:
- applies_to:
  - getUsagePolicy
  - listComparisons
  - getComparisonJson
  - getComparisonMarkdown
  - mcp
  description: 'No authentication, no API key, no signup: every format above is a plain GET on the public URL.'
  type: none
slug: comparefairly-com-authentication
source_filename: comparefairly-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://comparefairly.com/llms.txt\ndocs: https://comparefairly.com/llms.txt\nname: CompareFairly authentication\nschemes:\n- type: none\n  description: \"No authentication, no API key, no signup: every format above is a plain GET on the public URL.\"\n  applies_to: [getUsagePolicy, listComparisons, getComparisonJson, getComparisonMarkdown, mcp]\nnote: The provider OpenAPI (https://comparefairly.com/openapi.json) declares no securitySchemes, consistent with the llms.txt statement. The MCP endpoint POST /mcp is likewise described as public.\n"
source_yaml_url: https://artifacts.apis.io/comparefairly-com/authentication/comparefairly-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Comparison
- Artificial Intelligence
- Consumer Reviews
- Search
- MCP
- Open Data
- France
---
