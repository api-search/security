---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lorglabs-com-api-openapi.json
  format: json
  label: Lorg Check Api API
  slug: lorg-check-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lorglabs-com/openapi/_original/lorglabs-com-api-openapi.json
auth_types: []
description: Authentication schemes for Lorg Labs API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lorg Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lorg Labs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lorg Labs
provider_slug: lorglabs-com
scheme_count: 2
schemes:
- evidence: 'Header: `Authorization: Bearer lorg_…`, or `X-API-Key: lorg_…`.'
  header: Authorization
  how_to_obtain: Sign in with GitHub on https://lorglabs.com/get-a-key.md to receive a free key.
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'Header: `Authorization: Bearer lorg_…`, or `X-API-Key: lorg_…`.'
  header: X-API-Key
  how_to_obtain: Sign in with GitHub on https://lorglabs.com/get-a-key.md to receive a free key.
  location: header
  name: X-API-Key
  type: apiKey
slug: lorglabs-com-authentication
source_filename: lorglabs-com-authentication.yml
source_heading: Authentication Profile
source_url: https://lorglabs.com/docs-api-keys.md
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lorglabs.com/docs-api-keys.md\nsources:\n- https://lorglabs.com/docs-api-keys.md\n- https://lorglabs.com/docs-token-check.md\n- https://lorglabs.com/docs-quickstart.md\ndescription: Authentication schemes for Lorg Labs API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Header: `Authorization: Bearer lorg_…`, or `X-API-Key: lorg_…`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in with GitHub on https://lorglabs.com/get-a-key.md to receive a free key.\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Header: `Authorization: Bearer lorg_…`, or `X-API-Key: lorg_…`.'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Sign in with GitHub on https://lorglabs.com/get-a-key.md to receive a free key.\nnote: No OAuth2 flows are documented on the provided pages.\ndocs: https://lorglabs.com/docs-api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/lorglabs-com/authentication/lorglabs-com-authentication.yml
summary_line: 2 schemes
tags:
- Blockchain
- Safety
- Risk Assessment
- Automation
- Artificial Intelligence
---
