---
api_key_in: []
api_specs:
- filename: pangea-ai-guard-api-openapi.yml
  format: yaml
  label: Pangea AI Guard API
  slug: pangea-ai-guard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-ai-guard-api-openapi.yml
- filename: pangea-authn-api-openapi.yml
  format: yaml
  label: Pangea AuthN API
  slug: pangea-authn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-authn-api-openapi.yml
- filename: pangea-domain-intel-api-openapi.yml
  format: yaml
  label: Pangea Domain Intel API
  slug: pangea-domain-intel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-domain-intel-api-openapi.yml
- filename: pangea-file-scan-api-openapi.yml
  format: yaml
  label: Pangea File Scan API
  slug: pangea-file-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-file-scan-api-openapi.yml
- filename: pangea-ip-intel-api-openapi.yml
  format: yaml
  label: Pangea IP Intel API
  slug: pangea-ip-intel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-ip-intel-api-openapi.yml
- filename: pangea-redact-api-openapi.yml
  format: yaml
  label: Pangea Redact API
  slug: pangea-redact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-redact-api-openapi.yml
- filename: pangea-secure-audit-log-api-openapi.yml
  format: yaml
  label: Pangea Secure Audit Log API
  slug: pangea-secure-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-secure-audit-log-api-openapi.yml
- filename: pangea-vault-api-openapi.yml
  format: yaml
  label: Pangea Vault API
  slug: pangea-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pangea/refs/heads/main/openapi/pangea-vault-api-openapi.yml
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
