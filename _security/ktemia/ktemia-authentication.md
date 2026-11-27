---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ktemia-openapi-generated.yml
  format: yaml
  label: Ktemia API
  slug: ktemia-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ktemia/openapi/_ae-authored/ktemia-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ktemia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ktemia declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ktemia
provider_slug: ktemia
scheme_count: 1
schemes:
- evidence: 'Create a key in the dashboard . Send it on every call: X-API-Key: <your key>'
  header: X-API-Key
  how_to_obtain: Create a key in the dashboard
  location: header
  name: X-API-Key
  type: apiKey
slug: ktemia-authentication
source_filename: ktemia-authentication.yml
source_heading: Authentication Profile
source_url: https://www.ktemia.com/docs/getting-started/
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.ktemia.com/docs/getting-started/\nsources:\n- https://www.ktemia.com/docs/getting-started/\n- https://www.ktemia.com/docs/getting-started/\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Create a key in the dashboard . Send it on every call: X-API-Key: <your key>'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key in the dashboard\ndocs: https://www.ktemia.com/docs/getting-started/\n"
source_yaml_url: https://artifacts.apis.io/ktemia/authentication/ktemia-authentication.yml
summary_line: 1 scheme
tags:
- Travel
- Search
- Flights
- Hotels
- Cars
- Real Estate
---
