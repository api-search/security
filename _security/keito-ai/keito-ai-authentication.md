---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keito-ai-openapi-generated.yml
  format: yaml
  label: Keito API
  slug: keito-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keito-ai/openapi/_ae-authored/keito-ai-openapi-generated.yml
auth_types: []
description: Keito supports API key authentication and OAuth2 for the Make connector.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Keito Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keito declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Keito
provider_slug: keito-ai
scheme_count: 2
schemes:
- evidence: 'API key requests need both: Authorization: Bearer <kto_...> Keito-Account-Id: <company_id>'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API & Developers and copy the kto_... secret and the Company ID.
  name: API Key
  type: http-bearer
- evidence: The connector uses OAuth 2.0 authorization code through Keito’s identity provider, with openid profile email offline_access scopes and client_secret_basic token authentication.
  header: Authorization
  how_to_obtain: Obtain via the Make connector’s OAuth 2.0 authorization code flow managed by Make.
  name: Make OAuth
  scopes:
  - openid
  - profile
  - email
  - offline_access
  type: http-bearer
slug: keito-ai-authentication
source_filename: keito-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://keito.ai/docs/auth/api-keys/
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://keito.ai/docs/auth/api-keys/\nsources:\n- https://keito.ai/docs/auth/api-keys/\n- https://keito.ai/docs/api-reference/make/\n- https://keito.ai/docs/cli/authentication/\n- https://keito.ai/docs/security/okta-sso/\ndescription: Keito supports API key authentication and OAuth2 for the Make connector.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'API key requests need both: Authorization: Bearer <kto_...> Keito-Account-Id: <company_id>'\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API & Developers and copy the kto_... secret and the Company ID.\n- type: http-bearer\n  name: Make OAuth\n  evidence: The connector uses OAuth 2.0 authorization code through Keito’s identity provider, with openid profile email offline_access scopes\n    and client_secret_basic token authentication.\n  header: Authorization\n  scopes:\n  - openid\n  -\
  \ profile\n  - email\n  - offline_access\n  how_to_obtain: Obtain via the Make connector’s OAuth 2.0 authorization code flow managed by Make.\ndocs: https://keito.ai/docs/auth/api-keys/\n"
source_yaml_url: https://artifacts.apis.io/keito-ai/authentication/keito-ai-authentication.yml
summary_line: 2 schemes
tags:
- Time Tracking
- Invoicing
- Professional Services
- Artificial Intelligence
- London
---
