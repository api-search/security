---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: obeliskgate-com-account-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Account API
  slug: obeliskgate-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-account-api-openapi.yml
- filename: obeliskgate-com-agent-identity-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Agent Identity API
  slug: obeliskgate-com-agent-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-agent-identity-api-openapi.yml
- filename: obeliskgate-com-app-registration-api-openapi.yml
  format: yaml
  label: VaultSpark Studios App Registration API
  slug: obeliskgate-com-app-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-app-registration-api-openapi.yml
- filename: obeliskgate-com-auth-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Auth API
  slug: obeliskgate-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-auth-api-openapi.yml
- filename: obeliskgate-com-contact-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Contact API
  slug: obeliskgate-com-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-contact-api-openapi.yml
- filename: obeliskgate-com-email-verification-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Email Verification API
  slug: obeliskgate-com-email-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-email-verification-api-openapi.yml
- filename: obeliskgate-com-fedcm-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Fedcm API
  slug: obeliskgate-com-fedcm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-fedcm-api-openapi.yml
- filename: obeliskgate-com-federation-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Federation API
  slug: obeliskgate-com-federation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-federation-api-openapi.yml
- filename: obeliskgate-com-mcp-api-openapi.yml
  format: yaml
  label: VaultSpark Studios MCP API
  slug: obeliskgate-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-mcp-api-openapi.yml
- filename: obeliskgate-com-organizations-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Organizations API
  slug: obeliskgate-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-organizations-api-openapi.yml
- filename: obeliskgate-com-project-profile-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Project Profile API
  slug: obeliskgate-com-project-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-project-profile-api-openapi.yml
- filename: obeliskgate-com-proof-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Proof API
  slug: obeliskgate-com-proof-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-proof-api-openapi.yml
- filename: obeliskgate-com-release-history-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Release History API
  slug: obeliskgate-com-release-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-release-history-api-openapi.yml
- filename: obeliskgate-com-scan-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Scan API
  slug: obeliskgate-com-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-scan-api-openapi.yml
- filename: obeliskgate-com-seal-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Seal API
  slug: obeliskgate-com-seal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-seal-api-openapi.yml
- filename: obeliskgate-com-studio-ecosystem-api-openapi.yml
  format: yaml
  label: VaultSpark Studios Studio Ecosystem API
  slug: obeliskgate-com-studio-ecosystem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obeliskgate-com/openapi/obeliskgate-com-studio-ecosystem-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: VaultSpark Studios Authentication
name_suffix: Authentication
oauth_flows: []
overview: VaultSpark Studios secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VaultSpark Studios
provider_slug: obeliskgate-com
scheme_count: 2
schemes:
- description: obelisk_session cookie OR body.token
  in: cookie
  name: sessionCookie
  parameter: obelisk_session
  sources:
  - openapi/obeliskgate-com-openapi.json
  type: apiKey
- description: 'OIDC access token (Authorization: Bearer). Operations marked x-obelisk-auth:"owner" additionally require: session + org owner/admin.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/obeliskgate-com-openapi.json
  type: http
slug: obeliskgate-com-authentication
source_filename: obeliskgate-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/obeliskgate-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: obelisk_session\n  description: obelisk_session cookie OR body.token\n  sources:\n  - openapi/obeliskgate-com-openapi.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OIDC access token (Authorization: Bearer). Operations marked x-obelisk-auth:\"owner\"\n    additionally require: session + org owner/admin.'\n  sources:\n  - openapi/obeliskgate-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/obeliskgate-com/authentication/obeliskgate-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Authentication
- Security
- Identity
- Passkeys
- Artificial Intelligence
---
