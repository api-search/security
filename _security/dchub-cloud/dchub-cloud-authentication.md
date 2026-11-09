---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dchub-cloud-openapi.yml
  format: yaml
  label: DC Hub API
  slug: dc-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dchub-cloud/openapi/dchub-cloud-openapi.yml
- filename: dchub-cloud-api-openapi.json
  format: json
  label: DC Hub — Data Center Intelligence API API
  slug: dc-hub-data-center-intelligence-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dchub-cloud/openapi/_original/dchub-cloud-api-openapi.json
auth_types: []
description: Authentication for DC Hub uses an API key passed in a request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dchub Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: DC Hub declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DC Hub
provider_slug: dchub-cloud
scheme_count: 1
schemes:
- evidence: Your API key is the password that tells DC Hub it's you.
  header: X-API-Key
  how_to_obtain: The key is sent in a welcome email and can be viewed or re‑issued at dchub.cloud/developers after signing in.
  location: header
  name: API Key
  type: apiKey
slug: dchub-cloud-authentication
source_filename: dchub-cloud-authentication.yml
source_heading: Authentication Profile
source_url: https://dchub.cloud/guide
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dchub.cloud/guide\nsources:\n- https://dchub.cloud/guide\ndescription: Authentication for DC Hub uses an API key passed in a request header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Your API key is the password that tells DC Hub it's you.\n  location: header\n  header: X-API-Key\n  how_to_obtain: The key is sent in a welcome email and can be viewed or re‑issued at dchub.cloud/developers after signing in.\nnote: No OAuth2 or other authentication schemes are documented on the page.\ndocs: https://dchub.cloud/guide\n"
source_yaml_url: https://artifacts.apis.io/dchub-cloud/authentication/dchub-cloud-authentication.yml
summary_line: 1 scheme
tags:
- Data Center
- Power
- Infrastructure
- Open Data
---
