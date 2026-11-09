---
anonymous_access: false
api_key_in: []
api_specs:
- filename: finddoc-ca-clinics-api-openapi.yml
  format: yaml
  label: FindDoc Clinics API
  slug: finddoc-ca-clinics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-clinics-api-openapi.yml
- filename: finddoc-ca-doctors-api-openapi.yml
  format: yaml
  label: FindDoc Doctors API
  slug: finddoc-ca-doctors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-doctors-api-openapi.yml
- filename: finddoc-ca-health-api-openapi.yml
  format: yaml
  label: FindDoc Health API
  slug: finddoc-ca-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-health-api-openapi.yml
- filename: finddoc-ca-metadata-api-openapi.yml
  format: yaml
  label: FindDoc Metadata API
  slug: finddoc-ca-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-metadata-api-openapi.yml
- filename: finddoc-ca-specialists-api-openapi.yml
  format: yaml
  label: FindDoc Specialists API
  slug: finddoc-ca-specialists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-specialists-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Finddoc Ca Authentication
name_suffix: Authentication
oauth_flows: []
overview: FindDoc declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FindDoc
provider_slug: finddoc-ca
scheme_count: 2
schemes:
- evidence: Every request needs a Bearer token in the Authorization header.
  header: Authorization
  how_to_obtain: 'Use the published sandbox key or a paid API key and send it as "Authorization: Bearer <key>".'
  location: header
  name: Bearer token
  type: apiKey
- evidence: OAuth-capable hosts will discover the FindDoc login flow automatically when your account is eligible for hosted OAuth.
  how_to_obtain: Sign in with Google on the hosted MCP page; the MCP client receives a short-lived OAuth bearer token.
  name: Hosted MCP OAuth
  type: oauth2
slug: finddoc-ca-authentication
source_filename: finddoc-ca-authentication.yml
source_heading: Authentication Profile
source_url: https://www.finddoc.ca/developers/mcp
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.finddoc.ca/developers/mcp\nsources:\n- https://www.finddoc.ca/developers/mcp\n- https://www.finddoc.ca/developers\nschemes:\n- type: apiKey\n  name: Bearer token\n  evidence: Every request needs a Bearer token in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: 'Use the published sandbox key or a paid API key and send it as \"Authorization: Bearer <key>\".'\n- type: oauth2\n  name: Hosted MCP OAuth\n  evidence: OAuth-capable hosts will discover the FindDoc login flow automatically when your account is eligible for hosted OAuth.\n  how_to_obtain: Sign in with Google on the hosted MCP page; the MCP client receives a short-lived OAuth bearer token.\ndocs: https://www.finddoc.ca/developers/mcp\n"
source_yaml_url: https://artifacts.apis.io/finddoc-ca/authentication/finddoc-ca-authentication.yml
summary_line: 2 schemes
tags:
- Healthcare
- API
- Doctors
- Clinics
- Canada
---
