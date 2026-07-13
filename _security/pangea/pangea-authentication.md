---
api_key_in: []
api_specs:
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea AuthN API
  slug: authn
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea Secure Audit Log API
  slug: secure-audit-log
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea Redact API
  slug: redact
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea Vault API
  slug: vault
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea File Scan API
  slug: file-scan
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea IP Intel API
  slug: ip-intel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea Domain & URL Intel API
  slug: domain-intel
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
- filename: pangea-openapi.yml
  format: yaml
  label: Pangea AI Guard & Prompt Guard API
  slug: ai-guard
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Pangea Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pangea secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pangea
provider_slug: pangea
scheme_count: 1
schemes:
- description: Pangea service token or OAuth 2 access token passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/pangea-openapi.yml
  type: http
slug: pangea-authentication
source_filename: pangea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pangea-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Pangea service token or OAuth 2 access token passed as a Bearer token.\n  sources:\n  - openapi/pangea-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/authentication/pangea-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- AI Security
- Authentication
- Audit Log
- Data Protection
---
