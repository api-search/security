---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arcadiapower2-auth-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Auth API
  slug: arcadiapower2-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-auth-api-openapi.yml
- filename: arcadiapower2-bundle-beta-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Bundle (Beta) API
  slug: arcadiapower2-bundle-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-bundle-beta-api-openapi.yml
- filename: arcadiapower2-bundle-webhook-events-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Bundle Webhook Events API
  slug: arcadiapower2-bundle-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-bundle-webhook-events-api-openapi.yml
- filename: arcadiapower2-plug-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Plug API
  slug: arcadiapower2-plug-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-plug-api-openapi.yml
- filename: arcadiapower2-spark-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Spark API
  slug: arcadiapower2-spark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-spark-api-openapi.yml
- filename: arcadiapower2-users-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Users API
  slug: arcadiapower2-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-users-api-openapi.yml
- filename: arcadiapower2-utility-accounts-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Utility Accounts API
  slug: arcadiapower2-utility-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-utility-accounts-api-openapi.yml
- filename: arcadiapower2-utility-credentials-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Utility Credentials API
  slug: arcadiapower2-utility-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-utility-credentials-api-openapi.yml
- filename: arcadiapower2-utility-meters-beta-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Utility Meters (Beta) API
  slug: arcadiapower2-utility-meters-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-utility-meters-beta-api-openapi.yml
- filename: arcadiapower2-webhook-events-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Webhook Events API
  slug: arcadiapower2-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-webhook-events-api-openapi.yml
- filename: arcadiapower2-webhooks-api-openapi.yml
  format: yaml
  label: Arcadiapower2 Webhooks API
  slug: arcadiapower2-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/openapi/arcadiapower2-webhooks-api-openapi.yml
auth_types: []
description: Authentication for the Plug API uses OAuth2 with the client credentials flow.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Arcadiapower2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arcadiapower2 declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Arcadiapower2
provider_slug: arcadiapower2
scheme_count: 1
schemes:
- evidence: This API uses OAuth2 with the client credentials flow using the ['Create an Access Token'](https://docs.arcadia.com/reference/create-access-token) endpoint.
  flows:
  - client_credentials
  how_to_obtain: Retrieve an API key from the Dashboard and use it with the Create Access Token endpoint to obtain a time‑limited access token.
  name: OAuth2
  token_url: https://api.arcadia.com/oauth2/token
  type: oauth2
slug: arcadiapower2-authentication
source_filename: arcadiapower2-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.arcadia.com/docs/mfa.md
source_yaml: "generated: '2026-09-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.arcadia.com/docs/mfa.md\nsources:\n- https://docs.arcadia.com/docs/mfa.md\n- https://docs.arcadia.com/docs/api-authentication.md\n- https://docs.arcadia.com/reference/list-api-keys.md\n- https://docs.arcadia.com/reference/create-api-key.md\ndescription: Authentication for the Plug API uses OAuth2 with the client credentials flow.\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: This API uses OAuth2 with the client credentials flow using the ['Create an Access Token'](https://docs.arcadia.com/reference/create-access-token)\n    endpoint.\n  flows:\n  - client_credentials\n  token_url: https://api.arcadia.com/oauth2/token\n  how_to_obtain: Retrieve an API key from the Dashboard and use it with the Create Access Token endpoint to obtain a time‑limited access token.\nnote: No other authentication schemes (apiKey, http‑bearer, etc.) are documented for API calls.\n\
  docs: https://docs.arcadia.com/docs/mfa.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcadiapower2/refs/heads/main/authentication/arcadiapower2-authentication.yml
summary_line: 1 scheme
tags:
- Energy
- SaaS
- Enterprise
- Sustainability
- Data
---
