---
api_key_in: []
api_specs:
- filename: notte-openapi.yml
  format: yaml
  label: Notte Sessions API
  slug: sessions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-openapi.yml
- filename: notte-openapi.yml
  format: yaml
  label: Notte Agents API
  slug: agents
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-openapi.yml
- filename: notte-openapi.yml
  format: yaml
  label: Notte Page Observe / Step / Scrape API
  slug: page
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-openapi.yml
- filename: notte-openapi.yml
  format: yaml
  label: Notte Scraping API
  slug: scrape
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-openapi.yml
- filename: notte-openapi.yml
  format: yaml
  label: Notte Personas and Vaults API
  slug: personas-vaults
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Notte Authentication
name_suffix: Authentication
oauth_flows: []
overview: Notte secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Notte
provider_slug: notte
scheme_count: 1
schemes:
- description: Notte API key obtained from the Notte Console (https://console.notte.cc), passed as a Bearer token in the Authorization header. The SDK reads the NOTTE_API_KEY environment variable automatically.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/notte-openapi.yml
  type: http
slug: notte-authentication
source_filename: notte-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/notte-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Notte API key obtained from the Notte Console (https://console.notte.cc), passed\n    as a Bearer token in the Authorization header. The SDK reads the NOTTE_API_KEY environment\n    variable automatically.\n  sources:\n  - openapi/notte-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/authentication/notte-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Web Agents
- Browser Automation
- Sessions
- Scraping
---
