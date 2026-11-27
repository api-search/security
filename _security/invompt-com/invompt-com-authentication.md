---
anonymous_access: false
api_key_in: []
api_specs:
- filename: invompt-com-openapi-generated.yml
  format: yaml
  label: Invompt API
  slug: invompt-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invompt-com/openapi/_ae-authored/invompt-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for Invompt API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Invompt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Invompt declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Invompt
provider_slug: invompt-com
scheme_count: 2
schemes:
- evidence: 'The Invompt API uses Bearer token authentication. All requests must include an Authorization header:'
  header: Authorization
  how_to_obtain: OAuth is the default for a third‑party REST client acting on behalf of a user. The user approves access in the browser, the client receives an inv_at_ access token bound to the canonical /api/v1 resource.
  location: header
  name: OAuth 2.0
  scopes:
  - invoices:read
  - invoices:write
  - invoices:update
  - invoices:archive
  - invoices:send
  - clients:read
  - clients:write
  - settings:read
  - settings:write
  type: http-bearer
- evidence: API keys are intended for personal server‑side automations you own — cron jobs, internal tools, one‑off scripts.
  header: Authorization
  how_to_obtain: Create an API key at invompt.com/integrations under Developer automation, click New key, give it a name, and copy the key.
  location: header
  name: API Key
  type: http-bearer
slug: invompt-com-authentication
source_filename: invompt-com-authentication.yml
source_heading: Authentication Profile
source_url: https://invompt.com/docs/api/authentication
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://invompt.com/docs/api/authentication\nsources:\n- https://invompt.com/docs/api/authentication\ndescription: Authentication schemes for Invompt API\nschemes:\n- type: http-bearer\n  name: OAuth 2.0\n  evidence: 'The Invompt API uses Bearer token authentication. All requests must include an Authorization header:'\n  location: header\n  header: Authorization\n  scopes:\n  - invoices:read\n  - invoices:write\n  - invoices:update\n  - invoices:archive\n  - invoices:send\n  - clients:read\n  - clients:write\n  - settings:read\n  - settings:write\n  how_to_obtain: OAuth is the default for a third‑party REST client acting on behalf of a user. The user approves access in the browser, the client\n    receives an inv_at_ access token bound to the canonical /api/v1 resource.\n- type: http-bearer\n  name: API Key\n  evidence: API keys are intended for personal server‑side automations\
  \ you own — cron jobs, internal tools, one‑off scripts.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key at invompt.com/integrations under Developer automation, click New key, give it a name, and copy the key.\ndocs: https://invompt.com/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/invompt-com/authentication/invompt-com-authentication.yml
summary_line: 2 schemes
tags:
- Invoicing
- Artificial Intelligence
---
