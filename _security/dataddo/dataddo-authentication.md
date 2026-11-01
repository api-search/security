---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dataddo-openapi-generated.yml
  format: yaml
  label: Dataddo API
  slug: dataddo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataddo/openapi/_ae-authored/dataddo-openapi-generated.yml
auth_types: []
description: Authentication methods supported by Dataddo
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dataddo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dataddo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dataddo
provider_slug: dataddo
scheme_count: 2
schemes:
- evidence: OAuth 2.0 authorizers typically involve several steps, including registering your application with the data source, obtaining an access token, and refreshing the token as needed.
  flows:
  - App Flow
  - Authorization Code Flow
  - Refresh Token Flow
  how_to_obtain: Provide Client ID, Client Secret and Redirect URI (Authorization Code Flow) or use Dataddo‑generated URL (App Flow) as described in the documentation.
  name: OAuth 2.0
  type: oauth2
- evidence: Non-OAuth 2.0 authorizers only require to supply static values. Typically it is either a combination of a username and password or some static token or API key.
  how_to_obtain: Send required static fields (e.g., client_key, username, password) in the JSON payload to the /services endpoint.
  location: body
  name: Static credentials (non‑OAuth)
  type: apiKey
slug: dataddo-authentication
source_filename: dataddo-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.dataddo.com/headless/docs/creating-an-authorizer.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.dataddo.com/headless/docs/creating-an-authorizer.md\nsources:\n- https://docs.dataddo.com/headless/docs/creating-an-authorizer.md\n- https://docs.dataddo.com/headless/docs/authorizing-non-oauth-20-service.md\n- https://docs.dataddo.com/docs/securing-credentials.md\n- https://docs.dataddo.com/docs/securing-credentials\ndescription: Authentication methods supported by Dataddo\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: OAuth 2.0 authorizers typically involve several steps, including registering your application with the data source, obtaining an access\n    token, and refreshing the token as needed.\n  flows:\n  - App Flow\n  - Authorization Code Flow\n  - Refresh Token Flow\n  how_to_obtain: Provide Client ID, Client Secret and Redirect URI (Authorization Code Flow) or use Dataddo‑generated URL (App Flow) as described\n    in the documentation.\n- type:\
  \ apiKey\n  name: Static credentials (non‑OAuth)\n  evidence: Non-OAuth 2.0 authorizers only require to supply static values. Typically it is either a combination of a username and password or\n    some static token or API key.\n  location: body\n  how_to_obtain: Send required static fields (e.g., client_key, username, password) in the JSON payload to the /services endpoint.\ndocs: https://docs.dataddo.com/headless/docs/creating-an-authorizer.md\n"
source_yaml_url: https://artifacts.apis.io/dataddo/authentication/dataddo-authentication.yml
summary_line: 2 schemes
tags:
- Data Integration
- API Platform
- Artificial Intelligence
- Real-Time
- ETL
---
