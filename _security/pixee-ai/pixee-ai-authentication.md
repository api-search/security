---
api_key_in: []
api_specs:
- filename: pixee-ai-findings-api-openapi.yml
  format: yaml
  label: Pixee Findings API
  slug: pixee-ai-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixee-ai/refs/heads/main/openapi/pixee-ai-findings-api-openapi.yml
- filename: pixee-ai-fixes-api-openapi.yml
  format: yaml
  label: Pixee Fixes API
  slug: pixee-ai-fixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixee-ai/refs/heads/main/openapi/pixee-ai-fixes-api-openapi.yml
- filename: pixee-ai-repositories-api-openapi.yml
  format: yaml
  label: Pixee Repositories API
  slug: pixee-ai-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixee-ai/refs/heads/main/openapi/pixee-ai-repositories-api-openapi.yml
- filename: pixee-ai-scans-api-openapi.yml
  format: yaml
  label: Pixee Scans API
  slug: pixee-ai-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixee-ai/refs/heads/main/openapi/pixee-ai-scans-api-openapi.yml
- filename: pixee-ai-webhooks-api-openapi.yml
  format: yaml
  label: Pixee Webhooks API
  slug: pixee-ai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixee-ai/refs/heads/main/openapi/pixee-ai-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Pixee Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pixee declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Pixee
provider_slug: pixee-ai
scheme_count: 1
schemes:
- format: 'Authorization: Bearer <token>'
  header: Authorization
  id: bearerAuth
  location: header
  provisioning: Settings > API Tokens in the Pixee dashboard; token is displayed only once.
  scheme: bearer
  token_scope:
  - organization-wide
  - repository-specific
  type: http
slug: pixee-ai-authentication
source_filename: pixee-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.pixee.ai/api/overview\ndocs: https://docs.pixee.ai/api/overview\napi: Pixee REST API\nsummary: >-\n  Pixee uses bearer tokens for API authentication. Tokens are organization-scoped and\n  generated from Settings > API Tokens in the Pixee dashboard. Tokens can be\n  organization-wide or repository-specific. HTTPS/TLS is required for all requests.\nschemes:\n- id: bearerAuth\n  type: http\n  scheme: bearer\n  location: header\n  header: Authorization\n  format: \"Authorization: Bearer <token>\"\n  token_scope:\n  - organization-wide\n  - repository-specific\n  provisioning: Settings > API Tokens in the Pixee dashboard; token is displayed only once.\nbest_practices:\n- Rotate tokens every 90 days.\n- Use repository-scoped tokens for CI/CD pipelines that operate on a single repository.\n- Store tokens in a secrets manager (Vault, AWS Secrets Manager, GitHub Actions secrets).\n- Never commit tokens to source control.\n\
  enterprise:\n  sso: >-\n    Enterprise deployments support SSO for dashboard/user access with roles Admin,\n    Security Lead, and Member (see https://docs.pixee.ai/configuration/users).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixee-ai/refs/heads/main/authentication/pixee-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Security
- Application Security
- AppSec
- Vulnerability Remediation
- Static Analysis
- SARIF
- Code Security
- Artificial Intelligence
- Developer Tools
---
