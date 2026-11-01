---
anonymous_access: false
api_key_in: []
api_specs:
- filename: greencalculus-com-account-api-openapi.yml
  format: yaml
  label: greencalculus-com Account API
  slug: greencalculus-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/greencalculus-com/openapi/greencalculus-com-account-api-openapi.yml
- filename: greencalculus-com-bulk-api-openapi.yml
  format: yaml
  label: greencalculus-com Bulk API
  slug: greencalculus-com-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/greencalculus-com/openapi/greencalculus-com-bulk-api-openapi.yml
- filename: greencalculus-com-calculate-api-openapi.yml
  format: yaml
  label: greencalculus-com Calculate API
  slug: greencalculus-com-calculate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/greencalculus-com/openapi/greencalculus-com-calculate-api-openapi.yml
- filename: greencalculus-com-discovery-api-openapi.yml
  format: yaml
  label: greencalculus-com Discovery API
  slug: greencalculus-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/greencalculus-com/openapi/greencalculus-com-discovery-api-openapi.yml
- filename: greencalculus-com-factors-api-openapi.yml
  format: yaml
  label: greencalculus-com Factors API
  slug: greencalculus-com-factors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/greencalculus-com/openapi/greencalculus-com-factors-api-openapi.yml
auth_types: []
description: Authentication uses an API key provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Greencalculus Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: greencalculus-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: greencalculus-com
provider_slug: greencalculus-com
scheme_count: 1
schemes:
- evidence: A key unlocks the calculation engines and single-factor lookups.
  header: Authorization
  how_to_obtain: Get a free API key from the GreenCalculus dashboard ("Get a free API key" button).
  location: header
  name: Bearer
  type: http-bearer
slug: greencalculus-com-authentication
source_filename: greencalculus-com-authentication.yml
source_heading: Authentication Profile
source_url: https://greencalculus.com/developers/quickstart/
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://greencalculus.com/developers/quickstart/\nsources:\n- https://greencalculus.com/developers/quickstart/\n- https://greencalculus.com/guide-category/getting-started/\n- https://greencalculus.com/developers/tutorials/\ndescription: Authentication uses an API key provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: A key unlocks the calculation engines and single-factor lookups.\n  location: header\n  header: Authorization\n  how_to_obtain: Get a free API key from the GreenCalculus dashboard (\"Get a free API key\" button).\nnote: No OAuth2 flows, apiKey, or other authentication methods are documented on the provided pages.\ndocs: https://greencalculus.com/developers/quickstart/\n"
source_yaml_url: https://artifacts.apis.io/greencalculus-com/authentication/greencalculus-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Emissions
- API
- Data
- Sustainability
---
