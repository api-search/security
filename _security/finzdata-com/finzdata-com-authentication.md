---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for FinzData API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Finzdata Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: finzdata-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: finzdata-com
provider_slug: finzdata-com
scheme_count: 2
schemes:
- evidence: Authenticate with the X-API-Key header or the ?apikey= query parameter.
  header: X-API-Key
  how_to_obtain: Register at api.finzdata.com to obtain a free API key.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: Authenticate with the X-API-Key header or the ?apikey= query parameter.
  how_to_obtain: Register at api.finzdata.com to obtain a free API key.
  location: query
  name: apikey
  type: apiKey
slug: finzdata-com-authentication
source_filename: finzdata-com-authentication.yml
source_heading: Authentication Profile
source_url: https://finzdata.com/docs?ref=llms
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://finzdata.com/docs?ref=llms\nsources:\n- https://finzdata.com/docs?ref=llms\ndescription: Authentication methods for FinzData API\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Authenticate with the X-API-Key header or the ?apikey= query parameter.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Register at api.finzdata.com to obtain a free API key.\n- type: apiKey\n  name: apikey\n  evidence: Authenticate with the X-API-Key header or the ?apikey= query parameter.\n  location: query\n  how_to_obtain: Register at api.finzdata.com to obtain a free API key.\ndocs: https://finzdata.com/docs?ref=llms\n"
source_yaml_url: https://artifacts.apis.io/finzdata-com/authentication/finzdata-com-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Market Data
- Historical Data
- API
- Python
---
