---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keep-md-account-api-openapi.yml
  format: yaml
  label: Keep Account API
  slug: keep-md-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keep-md/openapi/keep-md-account-api-openapi.yml
- filename: keep-md-clients-and-tokens-api-openapi.yml
  format: yaml
  label: Keep Clients and tokens API
  slug: keep-md-clients-and-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keep-md/openapi/keep-md-clients-and-tokens-api-openapi.yml
- filename: keep-md-exports-api-openapi.yml
  format: yaml
  label: Keep Exports API
  slug: keep-md-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keep-md/openapi/keep-md-exports-api-openapi.yml
- filename: keep-md-highlights-api-openapi.yml
  format: yaml
  label: Keep Highlights API
  slug: keep-md-highlights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keep-md/openapi/keep-md-highlights-api-openapi.yml
- filename: keep-md-items-api-openapi.yml
  format: yaml
  label: Keep Items API
  slug: keep-md-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keep-md/openapi/keep-md-items-api-openapi.yml
- filename: keep-md-notes-api-openapi.yml
  format: yaml
  label: Keep Notes API
  slug: keep-md-notes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keep-md/openapi/keep-md-notes-api-openapi.yml
- filename: keep-md-projects-api-openapi.yml
  format: yaml
  label: Keep Projects API
  slug: keep-md-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keep-md/openapi/keep-md-projects-api-openapi.yml
- filename: keep-md-search-api-openapi.yml
  format: yaml
  label: Keep Search API
  slug: keep-md-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keep-md/openapi/keep-md-search-api-openapi.yml
- filename: keep-md-sources-api-openapi.yml
  format: yaml
  label: Keep Sources API
  slug: keep-md-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keep-md/openapi/keep-md-sources-api-openapi.yml
- filename: keep-md-tags-and-collections-api-openapi.yml
  format: yaml
  label: Keep Tags and collections API
  slug: keep-md-tags-and-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keep-md/openapi/keep-md-tags-and-collections-api-openapi.yml
- filename: keep-md-webhooks-api-openapi.yml
  format: yaml
  label: Keep Webhooks API
  slug: keep-md-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keep-md/openapi/keep-md-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for Keep API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Keep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keep declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Keep
provider_slug: keep-md
scheme_count: 1
schemes:
- evidence: 'Send it as a Bearer token:'
  header: Authorization
  how_to_obtain: Create a personal, connected, or read‑only API key in Keep settings and copy the key.
  location: header
  name: Bearer
  scopes:
  - profile
  - items.read
  - items.write
  - notes.read
  - notes.write
  - feed.read
  - feed.write
  - sources.read
  - sources.write
  type: http-bearer
slug: keep-md-authentication
source_filename: keep-md-authentication.yml
source_heading: Authentication Profile
source_url: https://keep.md/docs/api-keys.md
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://keep.md/docs/api-keys.md\nsources:\n- https://keep.md/docs/api-keys.md\n- https://keep.md/.well-known/oauth-protected-resource/mcp\n- https://keep.md/docs/api-keys\ndescription: Authentication schemes for Keep API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send it as a Bearer token:'\n  location: header\n  header: Authorization\n  scopes:\n  - profile\n  - items.read\n  - items.write\n  - notes.read\n  - notes.write\n  - feed.read\n  - feed.write\n  - sources.read\n  - sources.write\n  how_to_obtain: Create a personal, connected, or read‑only API key in Keep settings and copy the key.\ndocs: https://keep.md/docs/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/keep-md/authentication/keep-md-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Productivity
- Knowledge Management
- Markdown
- Automation
---
