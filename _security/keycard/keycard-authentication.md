---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keycard-keycard-api-api-openapi.yml
  format: yaml
  label: Keycard API
  slug: keycard-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keycard/openapi/keycard-keycard-api-api-openapi.yml
- filename: keycard-openapi-generated.yml
  format: yaml
  label: Keycard API
  slug: keycard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keycard/openapi/_ae-authored/keycard-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Keycard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keycard declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Keycard
provider_slug: keycard
scheme_count: 2
schemes:
- evidence: Keycard STS implements this using the authorization code flow with PKCE (OAuth 2.1).
  flows:
  - authorization_code
  how_to_obtain: The application redirects the user to Keycard STS, the user authenticates via the zone's identity provider, and the application exchanges the resulting authorization code for credentials.
  name: Keycard STS
  type: oauth2
- evidence: The application authenticates directly to Keycard STS using the client credentials flow (OAuth 2.1).
  flows:
  - client_credentials
  how_to_obtain: The application presents its client secret (or other supported application credential) to Keycard STS to obtain an access token.
  name: Keycard STS
  type: oauth2
slug: keycard-authentication
source_filename: keycard-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.keycard.ai/admin/zone-authentication.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.keycard.ai/admin/zone-authentication.md\nsources:\n- https://docs.keycard.ai/admin/zone-authentication.md\n- https://docs.keycard.ai/sdk/oauth.md\n- https://docs.keycard.ai/concepts/credentials.md\n- https://docs.keycard.ai/skills/keycard-credentials.md\nschemes:\n- type: oauth2\n  name: Keycard STS\n  evidence: Keycard STS implements this using the authorization code flow with PKCE (OAuth 2.1).\n  flows:\n  - authorization_code\n  how_to_obtain: The application redirects the user to Keycard STS, the user authenticates via the zone's identity provider, and the application\n    exchanges the resulting authorization code for credentials.\n- type: oauth2\n  name: Keycard STS\n  evidence: The application authenticates directly to Keycard STS using the client credentials flow (OAuth 2.1).\n  flows:\n  - client_credentials\n  how_to_obtain: The application presents its client\
  \ secret (or other supported application credential) to Keycard STS to obtain an access token.\ndocs: https://docs.keycard.ai/admin/zone-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/keycard/authentication/keycard-authentication.yml
summary_line: 2 schemes
tags:
- Authentication
- Authorization
- Identity
- Agent Security
- Policy as Code
- Runtime Access
---
