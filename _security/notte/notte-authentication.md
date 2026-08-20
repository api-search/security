---
api_key_in: []
api_specs:
- filename: notte-agents-api-openapi.yml
  format: yaml
  label: Notte Agents API
  slug: notte-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-agents-api-openapi.yml
- filename: notte-health-api-openapi.yml
  format: yaml
  label: Notte Health API
  slug: notte-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-health-api-openapi.yml
- filename: notte-page-api-openapi.yml
  format: yaml
  label: Notte Page API
  slug: notte-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-page-api-openapi.yml
- filename: notte-personas-api-openapi.yml
  format: yaml
  label: Notte Personas API
  slug: notte-personas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-personas-api-openapi.yml
- filename: notte-scraping-api-openapi.yml
  format: yaml
  label: Notte Scraping API
  slug: notte-scraping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-scraping-api-openapi.yml
- filename: notte-sessions-api-openapi.yml
  format: yaml
  label: Notte Sessions API
  slug: notte-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-sessions-api-openapi.yml
- filename: notte-vaults-api-openapi.yml
  format: yaml
  label: Notte Vaults API
  slug: notte-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/notte/refs/heads/main/openapi/notte-vaults-api-openapi.yml
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
- Artificial Intelligence
- Web Agents
- Browser Automation
- Sessions
- Scraping
---
