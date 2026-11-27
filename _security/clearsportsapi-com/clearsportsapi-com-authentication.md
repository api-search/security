---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clearsportsapi-com-openapi-generated.yml
  format: yaml
  label: ClearSports API
  slug: clearsportsapi-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearsportsapi-com/openapi/_ae-authored/clearsportsapi-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for ClearSports API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ClearSports Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClearSports declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ClearSports
provider_slug: clearsportsapi-com
scheme_count: 1
schemes:
- evidence: 'All protected endpoints require an API key passed in the Authorization header. Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  location: header
  name: API key (Bearer token)
  type: http-bearer
slug: clearsportsapi-com-authentication
source_filename: clearsportsapi-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.clearsportsapi.com/docs
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.clearsportsapi.com/docs\nsources:\n- https://www.clearsportsapi.com/docs\n- https://www.clearsportsapi.com/docs/playground?path=%2Fapi%2Fv1%2Fapi-keys%2Fme\ndescription: Authentication schemes for ClearSports API\nschemes:\n- type: http-bearer\n  name: API key (Bearer token)\n  evidence: 'All protected endpoints require an API key passed in the Authorization header. Authorization: Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\ndocs: https://www.clearsportsapi.com/docs\n"
source_yaml_url: https://artifacts.apis.io/clearsportsapi-com/authentication/clearsportsapi-com-authentication.yml
summary_line: 1 scheme
tags:
- Sports
- Data
- Betting
- Odds
---
