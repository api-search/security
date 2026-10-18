---
anonymous_access: false
api_key_in: []
api_specs:
- filename: burrow-events-api-openapi.yml
  format: yaml
  label: Burrow Events API
  slug: burrow-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burrow/refs/heads/main/openapi/burrow-events-api-openapi.yml
- filename: burrow-mcp-api-openapi.yml
  format: yaml
  label: Burrow MCP API
  slug: burrow-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/burrow/refs/heads/main/openapi/burrow-mcp-api-openapi.yml
auth_types: []
description: Authentication schemes as described on the Burrow documentation page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Burrow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Burrow declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Burrow
provider_slug: burrow
scheme_count: 2
schemes:
- evidence: Setup API key Create in Settings → Developer.
  header: Authorization
  how_to_obtain: Create in Settings → Developer.
  location: header
  name: Setup API key
  type: http-bearer
- evidence: Ingestion API key Separate keys for live event pipelines and CMS plugins.
  header: Authorization
  how_to_obtain: Separate keys for live event pipelines and CMS plugins.
  location: header
  name: Ingestion API key
  type: http-bearer
slug: burrow-authentication
source_filename: burrow-authentication.yml
source_heading: Authentication Profile
source_url: https://useburrow.com/docs
source_yaml: "generated: '2026-10-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://useburrow.com/docs\nsources:\n- https://useburrow.com/docs\ndescription: Authentication schemes as described on the Burrow documentation page.\nschemes:\n- type: http-bearer\n  name: Setup API key\n  evidence: Setup API key Create in Settings → Developer.\n  location: header\n  header: Authorization\n  how_to_obtain: Create in Settings → Developer.\n- type: http-bearer\n  name: Ingestion API key\n  evidence: Ingestion API key Separate keys for live event pipelines and CMS plugins.\n  location: header\n  header: Authorization\n  how_to_obtain: Separate keys for live event pipelines and CMS plugins.\ndocs: https://useburrow.com/docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/burrow/refs/heads/main/authentication/burrow-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Software-as-a-Service
- Reporting
- Automation
---
