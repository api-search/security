---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dealmachine-com-openapi-generated.yml
  format: yaml
  label: DealMachine API
  slug: dealmachine-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dealmachine-com/openapi/_ae-authored/dealmachine-com-openapi-generated.yml
auth_types: []
description: Authentication methods for DealMachine API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: DealMachine Authentication
name_suffix: Authentication
oauth_flows: []
overview: DealMachine declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DealMachine
provider_slug: dealmachine-com
scheme_count: 2
schemes:
- evidence: 'Include your API key in the `Authorization` header using the Bearer scheme:'
  header: Authorization
  how_to_obtain: Create keys via the Developer Settings page or by using the DealMachine CLI.
  location: header
  name: API Key
  type: http-bearer
- authorize_url: https://api.v2.dealmachine.com/v1/oauth/authorize
  evidence: 'The API also supports OAuth 2.0 access tokens for third‑party integrations:'
  how_to_obtain: Obtain a client_id (and optionally client_secret) from DealMachine developer settings, then follow the OAuth authorization code flow (or device flow via the CLI).
  name: OAuth 2.0
  scopes:
  - account:read
  token_url: https://api.v2.dealmachine.com/v1/oauth/token
  type: oauth2
slug: dealmachine-com-authentication
source_filename: dealmachine-com-authentication.yml
source_heading: Authentication Profile
source_url: https://api.docs.dealmachine.com/authentication.md
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.docs.dealmachine.com/authentication.md\nsources:\n- https://api.docs.dealmachine.com/authentication.md\n- https://api.docs.dealmachine.com/cli/authentication.md\n- https://api.docs.dealmachine.com/api-reference/oauth/authorize.md\n- https://api.docs.dealmachine.com/api-reference/oauth/token.md\ndescription: Authentication methods for DealMachine API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Include your API key in the `Authorization` header using the Bearer scheme:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys via the Developer Settings page or by using the DealMachine CLI.\n- type: oauth2\n  name: OAuth 2.0\n  evidence: 'The API also supports OAuth 2.0 access tokens for third‑party integrations:'\n  token_url: https://api.v2.dealmachine.com/v1/oauth/token\n  authorize_url: https://api.v2.dealmachine.com/v1/oauth/authorize\n\
  \  scopes:\n  - account:read\n  how_to_obtain: Obtain a client_id (and optionally client_secret) from DealMachine developer settings, then follow the OAuth authorization code\n    flow (or device flow via the CLI).\ndocs: https://api.docs.dealmachine.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/dealmachine-com/authentication/dealmachine-com-authentication.yml
summary_line: 2 schemes
tags:
- Real Estate
- Data
- Software-as-a-Service
- Lead Generation
- Property Search
---
