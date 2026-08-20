---
api_key_in: []
api_specs:
- filename: freestyle-sh-auth-api-openapi.yml
  format: yaml
  label: Freestyle Auth API
  slug: freestyle-sh-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-auth-api-openapi.yml
- filename: freestyle-sh-certs-api-openapi.yml
  format: yaml
  label: Freestyle Certs API
  slug: freestyle-sh-certs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-certs-api-openapi.yml
- filename: freestyle-sh-cron-api-openapi.yml
  format: yaml
  label: Freestyle Cron API
  slug: freestyle-sh-cron-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-cron-api-openapi.yml
- filename: freestyle-sh-dns-api-openapi.yml
  format: yaml
  label: Freestyle DNS API
  slug: freestyle-sh-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-dns-api-openapi.yml
- filename: freestyle-sh-domains-api-openapi.yml
  format: yaml
  label: Freestyle Domains API
  slug: freestyle-sh-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-domains-api-openapi.yml
- filename: freestyle-sh-execute-api-openapi.yml
  format: yaml
  label: Freestyle Execute API
  slug: freestyle-sh-execute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-execute-api-openapi.yml
- filename: freestyle-sh-git-api-openapi.yml
  format: yaml
  label: Freestyle Git API
  slug: freestyle-sh-git-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-git-api-openapi.yml
- filename: freestyle-sh-identity-api-openapi.yml
  format: yaml
  label: Freestyle Identity API
  slug: freestyle-sh-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-identity-api-openapi.yml
- filename: freestyle-sh-observability-api-openapi.yml
  format: yaml
  label: Freestyle Observability API
  slug: freestyle-sh-observability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-observability-api-openapi.yml
- filename: freestyle-sh-vm-api-openapi.yml
  format: yaml
  label: Freestyle VM API
  slug: freestyle-sh-vm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-vm-api-openapi.yml
- filename: freestyle-sh-web-api-openapi.yml
  format: yaml
  label: Freestyle Web API
  slug: freestyle-sh-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/openapi/freestyle-sh-web-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Freestyle Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Freestyle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Freestyle
provider_slug: freestyle-sh
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/freestyle-cron-api-openapi.yml
  - openapi/freestyle-domains-api-openapi.yml
  - openapi/freestyle-execute-api-openapi.yml
  - openapi/freestyle-git-api-openapi.yml
  - openapi/freestyle-identity-api-openapi.yml
  - openapi/freestyle-observability-api-openapi.yml
  - openapi/freestyle-vm-api-openapi.yml
  - openapi/freestyle-web-api-openapi.yml
  type: http
slug: freestyle-sh-authentication
source_filename: freestyle-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/freestyle-cron-api-openapi.yml, openapi/freestyle-domains-api-openapi.yml, openapi/freestyle-execute-api-openapi.yml,\n  openapi/freestyle-git-api-openapi.yml, openapi/freestyle-identity-api-openapi.yml, openapi/freestyle-observability-api-openapi.yml,\n  openapi/freestyle-vm-api-openapi.yml, openapi/freestyle-web-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/freestyle-cron-api-openapi.yml\n  - openapi/freestyle-domains-api-openapi.yml\n  - openapi/freestyle-execute-api-openapi.yml\n  - openapi/freestyle-git-api-openapi.yml\n  - openapi/freestyle-identity-api-openapi.yml\n  - openapi/freestyle-observability-api-openapi.yml\n  - openapi/freestyle-vm-api-openapi.yml\n  - openapi/freestyle-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freestyle-sh/refs/heads/main/authentication/freestyle-sh-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Agents
- Sandboxes
- VMs
- MicroVMs
- Git
- Code Execution
- JavaScript
- TypeScript
- Serverless
- Hosting
- Developer Tools
- Infrastructure
---
