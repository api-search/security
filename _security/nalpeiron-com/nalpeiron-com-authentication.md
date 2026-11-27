---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nalpeiron-com-openapi-generated.yml
  format: yaml
  label: Nalpeiron API
  slug: nalpeiron-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nalpeiron-com/openapi/_ae-authored/nalpeiron-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nalpeiron Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nalpeiron declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Nalpeiron
provider_slug: nalpeiron-com
scheme_count: 1
schemes:
- evidence: Request an OAuth access token from the Zenmeter API using your client credentials
  flows:
  - client_credentials
  how_to_obtain: Use the client ID and client secret from the Management API credentials page and POST to the token URL with grant_type=client_credentials
  name: client_credentials
  token_url: $NALPEIRON_TOKEN_URL
  type: oauth2
slug: nalpeiron-com-authentication
source_filename: nalpeiron-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.nalpeiron.com/zenmeter-docs/developers/api-quick-start/generate-an-oauth-token.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.nalpeiron.com/zenmeter-docs/developers/api-quick-start/generate-an-oauth-token.md\nsources:\n- https://docs.nalpeiron.com/zenmeter-docs/developers/api-quick-start/generate-an-oauth-token.md\n- https://docs.nalpeiron.com/zentitle2-docs/ui-administration/api-credentials.md\n- https://docs.nalpeiron.com/zentitle2-docs/ui-administration/api-credentials/package-registry.md\n- https://docs.nalpeiron.com/zentitle2-docs/ui-administration/configuration/account-based-licensing-identity-based-licensing/setup-account-based-licensing-with-openid-tokens.md\nschemes:\n- type: oauth2\n  name: client_credentials\n  evidence: Request an OAuth access token from the Zenmeter API using your client credentials\n  flows:\n  - client_credentials\n  token_url: $NALPEIRON_TOKEN_URL\n  how_to_obtain: Use the client ID and client secret from the Management API credentials page and POST to the\
  \ token URL with grant_type=client_credentials\ndocs: https://docs.nalpeiron.com/zenmeter-docs/developers/api-quick-start/generate-an-oauth-token.md\n"
source_yaml_url: https://artifacts.apis.io/nalpeiron-com/authentication/nalpeiron-com-authentication.yml
summary_line: 1 scheme
tags:
- Software Licensing
- Monetization
- Software-as-a-Service
- IoT
- Entitlement Management
---
