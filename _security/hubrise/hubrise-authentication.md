---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hubrise-openapi-generated.yml
  format: yaml
  label: HubRise API
  slug: hubrise-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubrise/openapi/_ae-authored/hubrise-openapi-generated.yml
auth_types: []
description: HubRise uses OAuth 2.0 for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hubrise Authentication
name_suffix: Authentication
oauth_flows: []
overview: HubRise declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: HubRise
provider_slug: hubrise
scheme_count: 1
schemes:
- authorize_url: https://manager.hubrise.com/oauth2/v1/authorize
  evidence: The HubRise API relies on the OAuth 2.0 protocol for this purpose.
  flows:
  - authorization_code
  how_to_obtain: Create an OAuth 2.0 client in the HubRise back‑office (Settings → Developer → Create an OAuth 2.0 client) and download the client secret JSON containing the client_id and client_secret.
  name: OAuth 2.0
  type: oauth2
slug: hubrise-authentication
source_filename: hubrise-authentication.yml
source_heading: Authentication Profile
source_url: https://www.hubrise.com/developers/api/authentication
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.hubrise.com/developers/api/authentication\nsources:\n- https://www.hubrise.com/developers/api/authentication\n- https://www.hubrise.com/developers\n- https://www.hubrise.com/developers/quick-start\ndescription: HubRise uses OAuth 2.0 for authentication.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: The HubRise API relies on the OAuth 2.0 protocol for this purpose.\n  flows:\n  - authorization_code\n  authorize_url: https://manager.hubrise.com/oauth2/v1/authorize\n  how_to_obtain: Create an OAuth 2.0 client in the HubRise back‑office (Settings → Developer → Create an OAuth 2.0 client) and download the client\n    secret JSON containing the client_id and client_secret.\nnote: Access tokens are obtained by POSTing to https://manager.hubrise.com/oauth2/v1/token with the client credentials and authorisation code.\ndocs: https://www.hubrise.com/developers/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/hubrise/authentication/hubrise-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Integration
- Retail
- Hospitality
- API
---
