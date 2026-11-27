---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dataville-com-connected-sheets-api-openapi.yml
  format: yaml
  label: Dataville Connected sheets API
  slug: dataville-com-connected-sheets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataville-com/openapi/dataville-com-connected-sheets-api-openapi.yml
- filename: dataville-com-data-sources-api-openapi.yml
  format: yaml
  label: Dataville Data sources API
  slug: dataville-com-data-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataville-com/openapi/dataville-com-data-sources-api-openapi.yml
- filename: dataville-com-export-and-sql-api-openapi.yml
  format: yaml
  label: Dataville Export and SQL API
  slug: dataville-com-export-and-sql-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataville-com/openapi/dataville-com-export-and-sql-api-openapi.yml
- filename: dataville-com-usage-api-openapi.yml
  format: yaml
  label: Dataville Usage API
  slug: dataville-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataville-com/openapi/dataville-com-usage-api-openapi.yml
auth_types: []
description: Dataville authenticates requests using an API key.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dataville Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dataville declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dataville
provider_slug: dataville-com
scheme_count: 2
schemes:
- evidence: Dataville's API authenticates using an API key.
  header: Authorization
  how_to_obtain: Create and manage your API key on the API Keys page of the dashboard; keys start with `dataville_`.
  location: header
  name: API Key
  type: apiKey
- evidence: 'These clients can pass the key in the `token` query parameter:'
  how_to_obtain: Create and manage your API key on the API Keys page of the dashboard; keys start with `dataville_`.
  location: query
  name: API Key (query)
  type: apiKey
slug: dataville-com-authentication
source_filename: dataville-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.dataville.com/api-reference/authentication.md
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.dataville.com/api-reference/authentication.md\nsources:\n- https://docs.dataville.com/api-reference/authentication.md\n- https://docs.dataville.com/quickstart-claude.md\n- https://docs.dataville.com/quickstart.md\n- https://docs.dataville.com/guides/onboarding-enrichment.md\ndescription: Dataville authenticates requests using an API key.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Dataville's API authenticates using an API key.\n  location: header\n  header: Authorization\n  how_to_obtain: Create and manage your API key on the API Keys page of the dashboard; keys start with `dataville_`.\n- type: apiKey\n  name: API Key (query)\n  evidence: 'These clients can pass the key in the `token` query parameter:'\n  location: query\n  how_to_obtain: Create and manage your API key on the API Keys page of the dashboard; keys start with `dataville_`.\nnote: Both schemes\
  \ use the same API key value.\ndocs: https://docs.dataville.com/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/dataville-com/authentication/dataville-com-authentication.yml
summary_line: 2 schemes
tags:
- Data API
- AI Applications
- Financial Filings
- Research Data
- Knowledge Attribution
---
