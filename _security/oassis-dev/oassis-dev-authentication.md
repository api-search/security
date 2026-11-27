---
anonymous_access: false
api_key_in: []
api_specs:
- filename: oassis-dev-account-api-openapi.yml
  format: yaml
  label: Oassis Account API
  slug: oassis-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oassis-dev/openapi/oassis-dev-account-api-openapi.yml
- filename: oassis-dev-agents-api-openapi.yml
  format: yaml
  label: Oassis Agents API
  slug: oassis-dev-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oassis-dev/openapi/oassis-dev-agents-api-openapi.yml
- filename: oassis-dev-discovery-api-openapi.yml
  format: yaml
  label: Oassis Discovery API
  slug: oassis-dev-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oassis-dev/openapi/oassis-dev-discovery-api-openapi.yml
- filename: oassis-dev-web-tasks-api-openapi.yml
  format: yaml
  label: Oassis Web Tasks API
  slug: oassis-dev-web-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oassis-dev/openapi/oassis-dev-web-tasks-api-openapi.yml
- filename: oassis-dev-web-tools-api-openapi.yml
  format: yaml
  label: Oassis Web Tools API
  slug: oassis-dev-web-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/oassis-dev/openapi/oassis-dev-web-tools-api-openapi.yml
auth_types: []
description: Authentication schemes for Oassis API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Oassis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oassis declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Oassis
provider_slug: oassis-dev
scheme_count: 1
schemes:
- evidence: 'curl -i https://api.oassis.dev/web/v1/scrape -H ''Authorization: Bearer YOUR_API_KEY'' -H ''Content-Type: application/json'' -d ''{"url":"https://example.com","formats":["markdown"]}'''
  header: Authorization
  how_to_obtain: Create an API key in your verified account.
  location: header
  name: API Key
  type: http-bearer
slug: oassis-dev-authentication
source_filename: oassis-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://oassis.dev/docs
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://oassis.dev/docs\nsources:\n- https://oassis.dev/docs\ndescription: Authentication schemes for Oassis API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'curl -i https://api.oassis.dev/web/v1/scrape -H ''Authorization: Bearer YOUR_API_KEY'' -H ''Content-Type: application/json'' -d ''{\"url\":\"https://example.com\",\"formats\":[\"markdown\"]}'''\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in your verified account.\ndocs: https://oassis.dev/docs\n"
source_yaml_url: https://artifacts.apis.io/oassis-dev/authentication/oassis-dev-authentication.yml
summary_line: 1 scheme
tags:
- Web Scraping
- Browser Automation
- AI Agents
- MCP
---
