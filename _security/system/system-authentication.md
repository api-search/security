---
anonymous_access: false
api_key_in: []
api_specs:
- filename: system-api-openapi.json
  format: json
  label: System REST API API
  slug: system-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/system/openapi/_original/system-api-openapi.json
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: System Authentication
name_suffix: Authentication
oauth_flows: []
overview: System declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: System
provider_slug: system
scheme_count: 1
schemes:
- evidence: 'All requests require your API key in the request header:'
  header: x-api-key
  how_to_obtain: Retrieve your API key from your beta portal page.
  location: header
  name: API Key
  type: apiKey
slug: system-authentication
source_filename: system-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.system.com/system/public/quick-start-guide.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.system.com/system/public/quick-start-guide.md\nsources:\n- https://docs.system.com/system/public/quick-start-guide.md\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'All requests require your API key in the request header:'\n  location: header\n  header: x-api-key\n  how_to_obtain: Retrieve your API key from your beta portal page.\ndocs: https://docs.system.com/system/public/quick-start-guide.md\n"
source_yaml_url: https://artifacts.apis.io/system/authentication/system-authentication.yml
summary_line: 1 scheme
tags:
- Healthcare
- Population Health
- Knowledge Graph
- API Platform
- Public Benefit Corporation
---
