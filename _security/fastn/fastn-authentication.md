---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fastn-fastn-api-api-openapi.yml
  format: yaml
  label: Fastn API
  slug: fastn-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastn/openapi/fastn-fastn-api-api-openapi.yml
- filename: fastn-openapi-generated.yml
  format: yaml
  label: Fastn API
  slug: fastn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastn/openapi/_ae-authored/fastn-openapi-generated.yml
auth_types: []
description: Fastn API keys authenticate requests using a Bearer token in the Authorization header. Test keys require an additional X‑fastn‑Test‑Mode header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fastn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fastn declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fastn
provider_slug: fastn
scheme_count: 1
schemes:
- evidence: Fastn API keys authenticate your backend's requests — including generating embed tokens.
  header: Authorization
  how_to_obtain: Create a key in Settings → API Keys; copy the displayed key (fsk_test_… or fsk_live_…).
  location: header
  name: Fastn API Key
  type: http-bearer
slug: fastn-authentication
source_filename: fastn-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fastn.ai/tutorials/developer/authentication-and-api-keys.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fastn.ai/tutorials/developer/authentication-and-api-keys.md\nsources:\n- https://docs.fastn.ai/tutorials/developer/authentication-and-api-keys.md\n- https://docs.fastn.ai/manage/api-keys.md\n- https://docs.fastn.ai/tutorials/developer/generating-embed-tokens.md\n- https://docs.fastn.ai/build/connectors/auth-methods.md\ndescription: Fastn API keys authenticate requests using a Bearer token in the Authorization header. Test keys require an additional X‑fastn‑Test‑Mode\n  header.\nschemes:\n- type: http-bearer\n  name: Fastn API Key\n  evidence: Fastn API keys authenticate your backend's requests — including generating embed tokens.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings → API Keys; copy the displayed key (fsk_test_… or fsk_live_…).\nnote: 'Test keys must also include the header \"X-fastn-Test-Mode: true\" as described on\
  \ the page.'\ndocs: https://docs.fastn.ai/tutorials/developer/authentication-and-api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/fastn/authentication/fastn-authentication.yml
summary_line: 1 scheme
tags:
- Integration Platform
- B2B SaaS
- Embedded Widget
- Unified API
- Data Integration
- AI Agents
- CRM Integration
- Security
---
