---
anonymous_access: false
api_key_in: []
api_specs:
- filename: credal-openapi-generated.yml
  format: yaml
  label: Credal API
  slug: credal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/credal/openapi/_ae-authored/credal-openapi-generated.yml
auth_types: []
description: Credal API v1 uses OAuth 2.0 Authorization Code flow with PKCE for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Credal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Credal declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Credal
provider_slug: credal
scheme_count: 1
schemes:
- authorize_url: https://app.credal.ai/api/oauth/authorize
  evidence: API v1 uses the OAuth 2.0 Authorization Code flow with **PKCE** (Proof Key for Code Exchange) for authentication.
  flows:
  - authorization_code
  how_to_obtain: Register an OAuth client with your organization’s admin (contact support@credal.ai) to receive a client ID and client secret.
  name: OAuth 2.0 Authorization Code with PKCE
  scopes:
  - api:agent:message:*
  type: oauth2
slug: credal-authentication
source_filename: credal-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.credal.ai/api-reference/v-1/o-auth-setup.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.credal.ai/api-reference/v-1/o-auth-setup.md\nsources:\n- https://docs.credal.ai/api-reference/v-1/o-auth-setup.md\n- https://docs.credal.ai/user-guide/platform/governed-actions/credentials-and-security\n- https://docs.credal.ai/api-reference/v-1/o-auth-setup\n- https://docs.credal.ai/user-guide/getting-started/introduction.md\ndescription: Credal API v1 uses OAuth 2.0 Authorization Code flow with PKCE for authentication.\nschemes:\n- type: oauth2\n  name: OAuth 2.0 Authorization Code with PKCE\n  evidence: API v1 uses the OAuth 2.0 Authorization Code flow with **PKCE** (Proof Key for Code Exchange) for authentication.\n  flows:\n  - authorization_code\n  authorize_url: https://app.credal.ai/api/oauth/authorize\n  scopes:\n  - api:agent:message:*\n  how_to_obtain: Register an OAuth client with your organization’s admin (contact support@credal.ai) to receive a client\
  \ ID and client secret.\ndocs: https://docs.credal.ai/api-reference/v-1/o-auth-setup.md\n"
source_yaml_url: https://artifacts.apis.io/credal/authentication/credal-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Platform
- Enterprise
- Automation
---
