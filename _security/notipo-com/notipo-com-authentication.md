---
anonymous_access: false
api_key_in: []
api_specs:
- filename: notipo-com-openapi-generated.yml
  format: yaml
  label: Notipo API
  slug: notipo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notipo-com/openapi/_ae-authored/notipo-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for Notipo API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Notipo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Notipo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Notipo
provider_slug: notipo-com
scheme_count: 1
schemes:
- evidence: All API requests require your API key in the X-API-Key header.
  header: X-API-Key
  how_to_obtain: Retrieve via Dashboard Settings → Account or programmatically via POST /api/auth/login which returns an apiKey.
  location: header
  name: API Key
  type: apiKey
slug: notipo-com-authentication
source_filename: notipo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://notipo.com/docs/api/introduction
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://notipo.com/docs/api/introduction\nsources:\n- https://notipo.com/docs/api/introduction\n- https://notipo.com/docs/getting-started\n- https://notipo.com/docs/wordpress-setup\n- https://notipo.com/docs/notion-setup\ndescription: Authentication schemes for Notipo API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: All API requests require your API key in the X-API-Key header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Retrieve via Dashboard Settings → Account or programmatically via POST /api/auth/login which returns an apiKey.\ndocs: https://notipo.com/docs/api/introduction\n"
source_yaml_url: https://artifacts.apis.io/notipo-com/authentication/notipo-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- WordPress
- Publishing
- Automation
- Integration
---
