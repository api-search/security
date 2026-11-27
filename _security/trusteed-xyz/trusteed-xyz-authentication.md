---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trusteed-xyz-openapi-generated.yml
  format: yaml
  label: Trusteed API
  slug: trusteed-xyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trusteed-xyz/openapi/_ae-authored/trusteed-xyz-openapi-generated.yml
auth_types: []
description: Authentication methods as documented on Trusteed developer page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Trusteed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trusteed declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Trusteed
provider_slug: trusteed-xyz
scheme_count: 2
schemes:
- evidence: 'Agent API Key (demo-store and sandbox) X-Agent-Api-Key: agnt_xxx For autonomous AI agents on demo-store and the REST agent API (/api/v1/agent/*).'
  header: X-Agent-Api-Key
  how_to_obtain: Create a key once via the Trusteed portal; use it without a session.
  location: header
  name: Agent API Key
  type: apiKey
- evidence: 'JWT Bearer Authorization: Bearer <token> For authenticated users. Obtain via POST /api/v1/auth/login.'
  header: Authorization
  how_to_obtain: POST https://trusteed.xyz/api/v1/auth/login with JSON body {"email":"you@example.com","password":"..."} to receive a JWT token.
  location: header
  name: JWT Bearer
  type: http-bearer
slug: trusteed-xyz-authentication
source_filename: trusteed-xyz-authentication.yml
source_heading: Authentication Profile
source_url: https://trusteed.xyz/en/developers
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://trusteed.xyz/en/developers\nsources:\n- https://trusteed.xyz/en/developers\ndescription: Authentication methods as documented on Trusteed developer page.\nschemes:\n- type: apiKey\n  name: Agent API Key\n  evidence: 'Agent API Key (demo-store and sandbox) X-Agent-Api-Key: agnt_xxx For autonomous AI agents on demo-store and the REST agent API (/api/v1/agent/*).'\n  location: header\n  header: X-Agent-Api-Key\n  how_to_obtain: Create a key once via the Trusteed portal; use it without a session.\n- type: http-bearer\n  name: JWT Bearer\n  evidence: 'JWT Bearer Authorization: Bearer <token> For authenticated users. Obtain via POST /api/v1/auth/login.'\n  location: header\n  header: Authorization\n  how_to_obtain: POST https://trusteed.xyz/api/v1/auth/login with JSON body {\"email\":\"you@example.com\",\"password\":\"...\"} to receive a JWT token.\nnote: OAuth 2.1 authentication\
  \ is mentioned but specific token or authorize URLs are not provided on the page, so no OAuth scheme is listed.\ndocs: https://trusteed.xyz/en/developers\n"
source_yaml_url: https://artifacts.apis.io/trusteed-xyz/authentication/trusteed-xyz-authentication.yml
summary_line: 2 schemes
tags:
- Agentic Commerce
- Store Audit
- Purchase Control
- E‑commerce Integration
---
