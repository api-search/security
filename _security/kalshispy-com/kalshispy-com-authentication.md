---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kalshispy-com-live-api-key-api-openapi.yml
  format: yaml
  label: KalshiSpy Live (API key) API
  slug: kalshispy-com-live-api-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kalshispy-com/openapi/kalshispy-com-live-api-key-api-openapi.yml
- filename: kalshispy-com-market-search-key-optional-api-openapi.yml
  format: yaml
  label: KalshiSpy Market search (key optional) API
  slug: kalshispy-com-market-search-key-optional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kalshispy-com/openapi/kalshispy-com-market-search-key-optional-api-openapi.yml
- filename: kalshispy-com-public-api-openapi.yml
  format: yaml
  label: KalshiSpy Public API
  slug: kalshispy-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kalshispy-com/openapi/kalshispy-com-public-api-openapi.yml
auth_types: []
description: Authentication uses a personal API token provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: KalshiSpy Authentication
name_suffix: Authentication
oauth_flows: []
overview: KalshiSpy declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: KalshiSpy
provider_slug: kalshispy-com
scheme_count: 1
schemes:
- evidence: Authentication → API Key · Auth Type Bearer · paste your ks_live_… token (create one in step 1 above).
  header: Authorization
  how_to_obtain: Create a personal API token in the KalshiSpy developer portal (step 1).
  location: header
  name: Bearer
  type: http-bearer
slug: kalshispy-com-authentication
source_filename: kalshispy-com-authentication.yml
source_heading: Authentication Profile
source_url: https://kalshispy.com/app/developers
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kalshispy.com/app/developers\nsources:\n- https://kalshispy.com/app/developers\ndescription: Authentication uses a personal API token provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Authentication → API Key · Auth Type Bearer · paste your ks_live_… token (create one in step 1 above).\n  location: header\n  header: Authorization\n  how_to_obtain: Create a personal API token in the KalshiSpy developer portal (step 1).\nnote: No other authentication methods (OAuth2, apiKey in query/body, etc.) are documented on the page.\ndocs: https://kalshispy.com/app/developers\n"
source_yaml_url: https://artifacts.apis.io/kalshispy-com/authentication/kalshispy-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Analytics
- Finance
- Prediction-Market
- Artificial Intelligence
---
