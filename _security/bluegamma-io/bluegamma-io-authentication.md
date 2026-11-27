---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for BlueGamma API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: BlueGamma Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlueGamma declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BlueGamma
provider_slug: bluegamma-io
scheme_count: 1
schemes:
- evidence: All BlueGamma API requests are authenticated with an API key that you issue yourself from the app.
  header: x-api-key
  how_to_obtain: Sign in at app.bluegamma.io, open API Keys in the sidebar, click Create API key, then copy the shown key.
  location: header
  name: API Key
  type: apiKey
slug: bluegamma-io-authentication
source_filename: bluegamma-io-authentication.yml
source_heading: Authentication Profile
source_url: https://www.bluegamma.io/documentation/integrations/api/authentication
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.bluegamma.io/documentation/integrations/api/authentication\nsources:\n- https://www.bluegamma.io/documentation/integrations/api/authentication\n- https://www.bluegamma.io/documentation\n- https://www.bluegamma.io/documentation/getting-started/setting-up-your-account\n- https://www.bluegamma.io/documentation/getting-started/installing-bluegamma-as-a-desktop-app\ndescription: Authentication methods for BlueGamma API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: All BlueGamma API requests are authenticated with an API key that you issue yourself from the app.\n  location: header\n  header: x-api-key\n  how_to_obtain: Sign in at app.bluegamma.io, open API Keys in the sidebar, click Create API key, then copy the shown key.\nnote: No OAuth2, HTTP Bearer, HTTP Basic, JWT, HMAC, mTLS, or other schemes are documented.\ndocs: https://www.bluegamma.io/documentation/integrations/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/bluegamma-io/authentication/bluegamma-io-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Market Data
- Interest Rates
- Company
---
