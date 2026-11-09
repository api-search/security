---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datasink-ing-documents-api-openapi.yml
  format: yaml
  label: DataSinking Documents API
  slug: datasink-ing-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-documents-api-openapi.yml
- filename: datasink-ing-exchanges-api-openapi.yml
  format: yaml
  label: DataSinking Exchanges API
  slug: datasink-ing-exchanges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-exchanges-api-openapi.yml
- filename: datasink-ing-feedback-api-openapi.yml
  format: yaml
  label: DataSinking Feedback API
  slug: datasink-ing-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-feedback-api-openapi.yml
- filename: datasink-ing-free-key-api-openapi.yml
  format: yaml
  label: DataSinking Free Key API
  slug: datasink-ing-free-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-free-key-api-openapi.yml
- filename: datasink-ing-stocks-api-openapi.yml
  format: yaml
  label: DataSinking Stocks API
  slug: datasink-ing-stocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datasink-ing/openapi/datasink-ing-stocks-api-openapi.yml
auth_types: []
description: Authentication is performed via a bearer token header or an API key query parameter.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Datasink Ing Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataSinking declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DataSinking
provider_slug: datasink-ing
scheme_count: 2
schemes:
- evidence: Auth is a bearer header, or ?apikey= in the URL for the clients that can't set one.
  header: Authorization
  how_to_obtain: Your API key is emailed to you the moment payment completes.
  location: header
  name: Bearer
  type: http-bearer
- evidence: Auth is a bearer header, or ?apikey= in the URL for the clients that can't set one.
  how_to_obtain: Your API key is emailed to you the moment payment completes.
  location: query
  name: apikey
  type: apiKey
slug: datasink-ing-authentication
source_filename: datasink-ing-authentication.yml
source_heading: Authentication Profile
source_url: https://datasink.ing/pricing
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://datasink.ing/pricing\nsources:\n- https://datasink.ing/pricing\n- https://datasink.ing/docs/mcp\ndescription: Authentication is performed via a bearer token header or an API key query parameter.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Auth is a bearer header, or ?apikey= in the URL for the clients that can't set one.\n  location: header\n  header: Authorization\n  how_to_obtain: Your API key is emailed to you the moment payment completes.\n- type: apiKey\n  name: apikey\n  evidence: Auth is a bearer header, or ?apikey= in the URL for the clients that can't set one.\n  location: query\n  how_to_obtain: Your API key is emailed to you the moment payment completes.\ndocs: https://datasink.ing/pricing\n"
source_yaml_url: https://artifacts.apis.io/datasink-ing/authentication/datasink-ing-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Reports
- Markdown
- Data
---
