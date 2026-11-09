---
anonymous_access: false
api_key_in: []
api_specs:
- filename: businessmcp-com-account-api-openapi.yml
  format: yaml
  label: BusinessMCP Account API
  slug: businessmcp-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-account-api-openapi.yml
- filename: businessmcp-com-assistant-api-openapi.yml
  format: yaml
  label: BusinessMCP Assistant API
  slug: businessmcp-com-assistant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-assistant-api-openapi.yml
- filename: businessmcp-com-companies-api-openapi.yml
  format: yaml
  label: BusinessMCP Companies API
  slug: businessmcp-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-companies-api-openapi.yml
- filename: businessmcp-com-email-api-openapi.yml
  format: yaml
  label: BusinessMCP Email API
  slug: businessmcp-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-email-api-openapi.yml
- filename: businessmcp-com-events-api-api-openapi.yml
  format: yaml
  label: BusinessMCP Events API
  slug: businessmcp-com-events-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-events-api-api-openapi.yml
- filename: businessmcp-com-export-api-openapi.yml
  format: yaml
  label: BusinessMCP Export API
  slug: businessmcp-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-export-api-openapi.yml
- filename: businessmcp-com-free-api-openapi.yml
  format: yaml
  label: BusinessMCP Free API
  slug: businessmcp-com-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-free-api-openapi.yml
- filename: businessmcp-com-ip-api-openapi.yml
  format: yaml
  label: BusinessMCP Ip API
  slug: businessmcp-com-ip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-ip-api-openapi.yml
- filename: businessmcp-com-meta-api-openapi.yml
  format: yaml
  label: BusinessMCP Meta API
  slug: businessmcp-com-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-meta-api-openapi.yml
- filename: businessmcp-com-people-api-openapi.yml
  format: yaml
  label: BusinessMCP People API
  slug: businessmcp-com-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-people-api-openapi.yml
- filename: businessmcp-com-read-api-api-openapi.yml
  format: yaml
  label: BusinessMCP Read API
  slug: businessmcp-com-read-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-read-api-api-openapi.yml
- filename: businessmcp-com-signup-api-openapi.yml
  format: yaml
  label: BusinessMCP Signup API
  slug: businessmcp-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-signup-api-openapi.yml
- filename: businessmcp-com-sites-api-openapi.yml
  format: yaml
  label: BusinessMCP Sites API
  slug: businessmcp-com-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-sites-api-openapi.yml
- filename: businessmcp-com-technology-api-openapi.yml
  format: yaml
  label: BusinessMCP Technology API
  slug: businessmcp-com-technology-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-technology-api-openapi.yml
- filename: businessmcp-com-tools-api-openapi.yml
  format: yaml
  label: BusinessMCP Tools API
  slug: businessmcp-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-tools-api-openapi.yml
- filename: businessmcp-com-traffic-api-openapi.yml
  format: yaml
  label: BusinessMCP Traffic API
  slug: businessmcp-com-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-traffic-api-openapi.yml
- filename: businessmcp-com-trust-api-openapi.yml
  format: yaml
  label: BusinessMCP Trust API
  slug: businessmcp-com-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-trust-api-openapi.yml
- filename: businessmcp-com-usage-api-openapi.yml
  format: yaml
  label: BusinessMCP Usage API
  slug: businessmcp-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-usage-api-openapi.yml
- filename: businessmcp-com-visibility-api-openapi.yml
  format: yaml
  label: BusinessMCP Visibility API
  slug: businessmcp-com-visibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/businessmcp-com/openapi/businessmcp-com-visibility-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Businessmcp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BusinessMCP secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BusinessMCP
provider_slug: businessmcp-com
scheme_count: 1
schemes:
- description: A BusinessMCP API key (mcph_…).
  name: bearer
  scheme: bearer
  sources:
  - openapi/businessmcp-com-hub-openapi.json
  - openapi/businessmcp-com-v1-openapi.json
  type: http
slug: businessmcp-com-authentication
source_filename: businessmcp-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/businessmcp-com-hub-openapi.json, openapi/businessmcp-com-v1-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: A BusinessMCP API key (mcph_…).\n  sources:\n  - openapi/businessmcp-com-hub-openapi.json\n  - openapi/businessmcp-com-v1-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/businessmcp-com/authentication/businessmcp-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Marketing
- Sales
- Automation
- Platform
---
