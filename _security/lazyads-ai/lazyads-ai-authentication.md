---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lazyads-ai-openapi-generated.yml
  format: yaml
  label: Lazy Ads API
  slug: lazyads-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lazyads-ai/openapi/_ae-authored/lazyads-ai-openapi-generated.yml
auth_types: []
description: Lazy Ads authenticates API requests using an API key that is sent either as a Bearer token in the Authorization header or as an X‑API‑Key header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lazy Ads Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lazy Ads declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lazy Ads
provider_slug: lazyads-ai
scheme_count: 2
schemes:
- evidence: 'Send Authorization: Bearer or X-API-Key on every request.'
  header: Authorization
  how_to_obtain: Generate an API key under Settings → API Keys; the key starts with "la_".
  name: Bearer token
  type: http-bearer
- evidence: Prefer the key inline, or the X-API-Key header?
  header: X-API-Key
  how_to_obtain: Generate an API key under Settings → API Keys; the key starts with "la_".
  name: X‑API‑Key header
  type: apiKey
slug: lazyads-ai-authentication
source_filename: lazyads-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://lazyads.ai/hermes
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lazyads.ai/hermes\nsources:\n- https://lazyads.ai/hermes\n- https://lazyads.ai/muse\ndescription: Lazy Ads authenticates API requests using an API key that is sent either as a Bearer token in the Authorization header or as an X‑API‑Key\n  header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Send Authorization: Bearer or X-API-Key on every request.'\n  header: Authorization\n  how_to_obtain: Generate an API key under Settings → API Keys; the key starts with \"la_\".\n- type: apiKey\n  name: X‑API‑Key header\n  evidence: Prefer the key inline, or the X-API-Key header?\n  header: X-API-Key\n  how_to_obtain: Generate an API key under Settings → API Keys; the key starts with \"la_\".\nnote: There is no OAuth2 flow, JWT, HMAC, MTLS, or other authentication method documented.\ndocs: https://lazyads.ai/hermes\n"
source_yaml_url: https://artifacts.apis.io/lazyads-ai/authentication/lazyads-ai-authentication.yml
summary_line: 2 schemes
tags:
- Advertising
- Artificial Intelligence
- Marketing
- Automation
- Software-as-a-Service
---
