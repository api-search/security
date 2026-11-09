---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aginera-ai-billing-api-openapi.yml
  format: yaml
  label: Aginera Billing API
  slug: aginera-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-billing-api-openapi.yml
- filename: aginera-ai-cad-api-openapi.yml
  format: yaml
  label: Aginera CAD API
  slug: aginera-ai-cad-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-cad-api-openapi.yml
- filename: aginera-ai-clients-api-openapi.yml
  format: yaml
  label: Aginera Clients API
  slug: aginera-ai-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-clients-api-openapi.yml
- filename: aginera-ai-documents-api-openapi.yml
  format: yaml
  label: Aginera Documents API
  slug: aginera-ai-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-documents-api-openapi.yml
- filename: aginera-ai-exports-api-openapi.yml
  format: yaml
  label: Aginera Exports API
  slug: aginera-ai-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-exports-api-openapi.yml
- filename: aginera-ai-projects-api-openapi.yml
  format: yaml
  label: Aginera Projects API
  slug: aginera-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-projects-api-openapi.yml
- filename: aginera-ai-reference-api-openapi.yml
  format: yaml
  label: Aginera Reference API
  slug: aginera-ai-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-reference-api-openapi.yml
- filename: aginera-ai-takeoffs-api-openapi.yml
  format: yaml
  label: Aginera Takeoffs API
  slug: aginera-ai-takeoffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-takeoffs-api-openapi.yml
- filename: aginera-ai-usage-api-openapi.yml
  format: yaml
  label: Aginera Usage API
  slug: aginera-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aginera-ai/openapi/aginera-ai-usage-api-openapi.yml
auth_types: []
description: Authentication methods for Aginera APIs
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Aginera Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aginera declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Aginera
provider_slug: aginera-ai
scheme_count: 3
schemes:
- evidence: 'A static key ( agk_… ) sent as Authorization: Bearer'
  header: Authorization
  how_to_obtain: Create a key in Settings → API (admin only) and copy the shown agk_… value
  location: header
  name: API key
  type: http-bearer
- authorize_url: https://auth.aginera.ai/oauth/authorize
  evidence: OAuth 2.1 authorization code + PKCE, with refresh tokens https://auth.aginera.ai
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Register a public client at the registration endpoint (no client secret) and run the authorization code flow with PKCE
  location: header
  name: Delegated OAuth
  scopes:
  - projects:read/write/delete
  - documents:read/write/delete
  - takeoffs:read/run/review/delete
  - exports:read/create
  - estimates:read/generate
  - billing:read/write
  - events:read
  - webhooks:manage
  type: oauth2
- evidence: OAuth 2.0 client credentials, issued by Microsoft Entra ID.
  flows:
  - client_credentials
  header: Authorization
  how_to_obtain: Provision client_id and client_secret during partner onboarding (email developers@aginera.ai) and request a token from Microsoft Entra
  location: header
  name: Service credentials (Entra)
  scopes:
  - api://$AGINERA_API_APP_ID/.default
  token_url: https://login.microsoftonline.com/$AGINERA_TENANT_ID/oauth2/v2.0/token
  type: oauth2
slug: aginera-ai-authentication
source_filename: aginera-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://aginera.ai/docs/developer/authentication
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://aginera.ai/docs/developer/authentication\nsources:\n- https://aginera.ai/docs/developer/authentication\n- https://aginera.ai/docs/getting-started\n- https://aginera.ai/docs/developer/rest-quickstart\n- https://aginera.ai/docs/guides/user-manual/onboarding\ndescription: Authentication methods for Aginera APIs\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'A static key ( agk_… ) sent as Authorization: Bearer'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings → API (admin only) and copy the shown agk_… value\n- type: oauth2\n  name: Delegated OAuth\n  evidence: OAuth 2.1 authorization code + PKCE, with refresh tokens https://auth.aginera.ai\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://auth.aginera.ai/oauth/authorize\n  scopes:\n  - projects:read/write/delete\n  -\
  \ documents:read/write/delete\n  - takeoffs:read/run/review/delete\n  - exports:read/create\n  - estimates:read/generate\n  - billing:read/write\n  - events:read\n  - webhooks:manage\n  how_to_obtain: Register a public client at the registration endpoint (no client secret) and run the authorization code flow with PKCE\n- type: oauth2\n  name: Service credentials (Entra)\n  evidence: OAuth 2.0 client credentials, issued by Microsoft Entra ID.\n  location: header\n  header: Authorization\n  flows:\n  - client_credentials\n  token_url: https://login.microsoftonline.com/$AGINERA_TENANT_ID/oauth2/v2.0/token\n  scopes:\n  - api://$AGINERA_API_APP_ID/.default\n  how_to_obtain: Provision client_id and client_secret during partner onboarding (email developers@aginera.ai) and request a token from Microsoft\n    Entra\ndocs: https://aginera.ai/docs/developer/authentication\n"
source_yaml_url: https://artifacts.apis.io/aginera-ai/authentication/aginera-ai-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Construction
- Estimating
- MEP
- Software
---
