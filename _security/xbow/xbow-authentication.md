---
api_key_in: []
api_specs:
- filename: xbow-assessments-api-openapi.yml
  format: yaml
  label: Xbow Assessments API
  slug: xbow-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-assessments-api-openapi.yml
- filename: xbow-assets-api-openapi.yml
  format: yaml
  label: Xbow Assets API
  slug: xbow-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-assets-api-openapi.yml
- filename: xbow-findings-api-openapi.yml
  format: yaml
  label: Xbow Findings API
  slug: xbow-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-findings-api-openapi.yml
- filename: xbow-lightspeed-api-openapi.yml
  format: yaml
  label: Xbow Lightspeed API
  slug: xbow-lightspeed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-lightspeed-api-openapi.yml
- filename: xbow-meta-api-openapi.yml
  format: yaml
  label: Xbow Meta API
  slug: xbow-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-meta-api-openapi.yml
- filename: xbow-organizations-api-openapi.yml
  format: yaml
  label: Xbow Organizations API
  slug: xbow-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-organizations-api-openapi.yml
- filename: xbow-reports-api-openapi.yml
  format: yaml
  label: Xbow Reports API
  slug: xbow-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-reports-api-openapi.yml
- filename: xbow-resources-api-openapi.yml
  format: yaml
  label: Xbow Resources API
  slug: xbow-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-resources-api-openapi.yml
- filename: xbow-webhooks-api-openapi.yml
  format: yaml
  label: Xbow Webhooks API
  slug: xbow-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/openapi/xbow-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Xbow Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xbow secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Xbow
provider_slug: xbow
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: Authorization header with Bearer token
  name: Authorization
  scheme: bearer
  sources:
  - openapi/xbow-openapi-original.json
  type: http
slug: xbow-authentication
source_filename: xbow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/xbow-openapi-original.json\ndocs: https://docs.xbow.com/api/#description/accessing-the-api\nsummary:\n  types:\n  - http\n  scheme: bearer personal access token (PAT)\nschemes:\n- name: Authorization\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Authorization header with Bearer token\n  sources:\n  - openapi/xbow-openapi-original.json\ndetails:\n  token_type: Personal Access Token, organization-scoped\n  issuance: Console (console.xbow.com) > profile > Settings > Personal Access Tokens >\n    Generate new token; requires organization administrator access; shown once.\n  organization_keys: POST /api/v1/organizations/{organizationId}/keys creates org keys;\n    DELETE /api/v1/keys/{keyId} revokes them.\n  required_headers:\n  - 'Authorization: Bearer <token>'\n  - 'X-XBOW-API-Version: <YYYY-MM-DD>'\n  restrictions: Lightspeed organizations get read-only API access (GET endpoints only).\n  guidance:\
  \ Store keys in env vars/secret managers, never commit to version control,\n    rotate periodically, revoke compromised keys immediately.\n  console_sso: SSO/SCIM available for Console user auth via customer IdP (Enterprise);\n    not an API auth surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xbow/refs/heads/main/authentication/xbow-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- Penetration Testing
- Offensive Security
- Artificial Intelligence
- Vulnerability Management
- Cybersecurity
- Application Security
---
