---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coherent-global-openapi-generated.yml
  format: yaml
  label: Coherent API
  slug: coherent-global-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coherent-global/openapi/_ae-authored/coherent-global-openapi-generated.yml
auth_types: []
description: Authentication methods published by Coherent
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Coherent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coherent declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Coherent
provider_slug: coherent-global
scheme_count: 2
schemes:
- evidence: The client credentials grant feature of OAuth 2.0 enables server-to-server authentication, without involving actual users.
  flows:
  - client_credentials
  how_to_obtain: Create a client in the Keycloak console, copy the client secret and client ID, then request a token via the token endpoint using grant_type=client_credentials.
  name: Client Credentials
  token_url: https://keycloak.{environment}.coherent.global/auth/realms/{tenant}/protocol/openid-connect/token
  type: oauth2
- evidence: 'For APIs that accept API keys, the request header must include: `x-synthetic-key` for the API key.'
  header: x-synthetic-key
  how_to_obtain: Tenant‑admin creates an API key in the Spark UI (New API key button) and copies the generated key.
  location: header
  name: API Key
  type: apiKey
slug: coherent-global-authentication
source_filename: coherent-global-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.coherent.global/identity-and-access-management/client-credentials/benefits-of-client-credentials-versus-api-keys.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.coherent.global/identity-and-access-management/client-credentials/benefits-of-client-credentials-versus-api-keys.md\nsources:\n- https://docs.coherent.global/identity-and-access-management/client-credentials/benefits-of-client-credentials-versus-api-keys.md\n- https://docs.coherent.global/identity-and-access-management/client-credentials/client-credentials-grant-oauth-2.0.md\n- https://docs.coherent.global/spark-apis/authorization-api-keys.md\n- https://docs.coherent.global/spark-apis/authorization-api-keys/permissions-features-permissions.md\ndescription: Authentication methods published by Coherent\nschemes:\n- type: oauth2\n  name: Client Credentials\n  evidence: The client credentials grant feature of OAuth 2.0 enables server-to-server authentication, without involving actual users.\n  flows:\n  - client_credentials\n  token_url: https://keycloak.{environment}.coherent.global/auth/realms/{tenant}/protocol/openid-connect/token\n\
  \  how_to_obtain: Create a client in the Keycloak console, copy the client secret and client ID, then request a token via the token endpoint using\n    grant_type=client_credentials.\n- type: apiKey\n  name: API Key\n  evidence: 'For APIs that accept API keys, the request header must include: `x-synthetic-key` for the API key.'\n  location: header\n  header: x-synthetic-key\n  how_to_obtain: Tenant‑admin creates an API key in the Spark UI (New API key button) and copies the generated key.\ndocs: https://docs.coherent.global/identity-and-access-management/client-credentials/benefits-of-client-credentials-versus-api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/coherent-global/authentication/coherent-global-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Excel
- Automation
- Insurance
- Finance
---
