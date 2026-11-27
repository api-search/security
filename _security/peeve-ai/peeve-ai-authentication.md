---
anonymous_access: false
api_key_in: []
api_specs:
- filename: peeve-ai-analytics-api-openapi.yml
  format: yaml
  label: Peeve Analytics API
  slug: peeve-ai-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peeve-ai/openapi/peeve-ai-analytics-api-openapi.yml
- filename: peeve-ai-ask-api-openapi.yml
  format: yaml
  label: Peeve Ask API
  slug: peeve-ai-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peeve-ai/openapi/peeve-ai-ask-api-openapi.yml
- filename: peeve-ai-configuration-api-openapi.yml
  format: yaml
  label: Peeve Configuration API
  slug: peeve-ai-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peeve-ai/openapi/peeve-ai-configuration-api-openapi.yml
- filename: peeve-ai-contacts-api-openapi.yml
  format: yaml
  label: Peeve Contacts API
  slug: peeve-ai-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peeve-ai/openapi/peeve-ai-contacts-api-openapi.yml
- filename: peeve-ai-hand-offs-api-openapi.yml
  format: yaml
  label: Peeve Hand Offs API
  slug: peeve-ai-hand-offs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peeve-ai/openapi/peeve-ai-hand-offs-api-openapi.yml
- filename: peeve-ai-leads-api-openapi.yml
  format: yaml
  label: Peeve Leads API
  slug: peeve-ai-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peeve-ai/openapi/peeve-ai-leads-api-openapi.yml
- filename: peeve-ai-meetings-api-openapi.yml
  format: yaml
  label: Peeve Meetings API
  slug: peeve-ai-meetings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peeve-ai/openapi/peeve-ai-meetings-api-openapi.yml
- filename: peeve-ai-sessions-api-openapi.yml
  format: yaml
  label: Peeve Sessions API
  slug: peeve-ai-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peeve-ai/openapi/peeve-ai-sessions-api-openapi.yml
- filename: peeve-ai-users-api-openapi.yml
  format: yaml
  label: Peeve Users API
  slug: peeve-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peeve-ai/openapi/peeve-ai-users-api-openapi.yml
- filename: peeve-ai-webhooks-api-openapi.yml
  format: yaml
  label: Peeve Webhooks API
  slug: peeve-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/peeve-ai/openapi/peeve-ai-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for Peeve API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Peeve Authentication
name_suffix: Authentication
oauth_flows: []
overview: Peeve declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Peeve
provider_slug: peeve-ai
scheme_count: 3
schemes:
- evidence: 'Secret key — as a bearer token, or in the Peeve header:'
  header: Authorization
  how_to_obtain: Created in the dashboard under Settings → API keys as a secret key.
  location: header
  name: Secret key Bearer token
  type: http-bearer
- evidence: 'Secret key — as a bearer token, or in the Peeve header:'
  header: X-Peeve-Key
  how_to_obtain: Created in the dashboard under Settings → API keys as a secret key.
  location: header
  name: Secret key header
  type: apiKey
- evidence: 'Publishable key — you do not normally send this yourself. It goes in your widget script tag, and the widget handles the rest:'
  how_to_obtain: Created in the dashboard under Settings → API keys as a publishable key.
  location: script tag attribute
  name: Publishable key
  type: other
slug: peeve-ai-authentication
source_filename: peeve-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.peeve.ai/authentication/overview.md
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.peeve.ai/authentication/overview.md\nsources:\n- https://docs.peeve.ai/authentication/overview.md\n- https://docs.peeve.ai/authentication/credentials.md\n- https://docs.peeve.ai/authentication/roles.md\n- https://docs.peeve.ai/authentication/keys.md\ndescription: Authentication schemes for Peeve API\nschemes:\n- type: http-bearer\n  name: Secret key Bearer token\n  evidence: 'Secret key — as a bearer token, or in the Peeve header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Created in the dashboard under Settings → API keys as a secret key.\n- type: apiKey\n  name: Secret key header\n  evidence: 'Secret key — as a bearer token, or in the Peeve header:'\n  location: header\n  header: X-Peeve-Key\n  how_to_obtain: Created in the dashboard under Settings → API keys as a secret key.\n- type: other\n  name: Publishable key\n  evidence: 'Publishable key\
  \ — you do not normally send this yourself. It goes in your widget script tag, and the widget handles the rest:'\n  location: script tag attribute\n  how_to_obtain: Created in the dashboard under Settings → API keys as a publishable key.\ndocs: https://docs.peeve.ai/authentication/overview.md\nnote: 2 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/peeve-ai/authentication/peeve-ai-authentication.yml
summary_line: 3 schemes
tags:
- AI Customer Support
- Software-as-a-Service
- In‑app Help
- Backend Integration
- Analytics
---
