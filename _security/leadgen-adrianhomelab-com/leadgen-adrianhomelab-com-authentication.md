---
anonymous_access: false
api_key_in: []
api_specs:
- filename: leadgen-adrianhomelab-com-account-api-openapi.yml
  format: yaml
  label: Leadgen (Romanian company data) Account API
  slug: leadgen-adrianhomelab-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadgen-adrianhomelab-com/openapi/leadgen-adrianhomelab-com-account-api-openapi.yml
- filename: leadgen-adrianhomelab-com-alerts-api-openapi.yml
  format: yaml
  label: Leadgen (Romanian company data) Alerts API
  slug: leadgen-adrianhomelab-com-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadgen-adrianhomelab-com/openapi/leadgen-adrianhomelab-com-alerts-api-openapi.yml
- filename: leadgen-adrianhomelab-com-billing-api-openapi.yml
  format: yaml
  label: Leadgen (Romanian company data) Billing API
  slug: leadgen-adrianhomelab-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadgen-adrianhomelab-com/openapi/leadgen-adrianhomelab-com-billing-api-openapi.yml
- filename: leadgen-adrianhomelab-com-feedback-api-openapi.yml
  format: yaml
  label: Leadgen (Romanian company data) Feedback API
  slug: leadgen-adrianhomelab-com-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadgen-adrianhomelab-com/openapi/leadgen-adrianhomelab-com-feedback-api-openapi.yml
- filename: leadgen-adrianhomelab-com-free-key-api-openapi.yml
  format: yaml
  label: Leadgen (Romanian company data) Free key API
  slug: leadgen-adrianhomelab-com-free-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadgen-adrianhomelab-com/openapi/leadgen-adrianhomelab-com-free-key-api-openapi.yml
- filename: leadgen-adrianhomelab-com-lookups-api-openapi.yml
  format: yaml
  label: Leadgen (Romanian company data) Lookups API
  slug: leadgen-adrianhomelab-com-lookups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadgen-adrianhomelab-com/openapi/leadgen-adrianhomelab-com-lookups-api-openapi.yml
- filename: leadgen-adrianhomelab-com-watchlist-api-openapi.yml
  format: yaml
  label: Leadgen (Romanian company data) Watchlist API
  slug: leadgen-adrianhomelab-com-watchlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadgen-adrianhomelab-com/openapi/leadgen-adrianhomelab-com-watchlist-api-openapi.yml
auth_types: []
description: Authentication uses an API key that can be sent either in the X-API-Key header or as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Leadgen (Romanian company data) Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leadgen (Romanian company data) declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Leadgen (Romanian company data)
provider_slug: leadgen-adrianhomelab-com
scheme_count: 2
schemes:
- evidence: 'Send the key in the X-API-Key header or as Authorization: Bearer .'
  header: X-API-Key
  how_to_obtain: Sign in with Google or with your email.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Send the key in the X-API-Key header or as Authorization: Bearer .'
  header: Authorization
  how_to_obtain: Sign in with Google or with your email.
  location: header
  name: Authorization
  type: http-bearer
slug: leadgen-adrianhomelab-com-authentication
source_filename: leadgen-adrianhomelab-com-authentication.yml
source_heading: Authentication Profile
source_url: https://leadgen-api.adrianhomelab.com/en/start
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://leadgen-api.adrianhomelab.com/en/start\nsources:\n- https://leadgen-api.adrianhomelab.com/en/start\ndescription: Authentication uses an API key that can be sent either in the X-API-Key header or as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Send the key in the X-API-Key header or as Authorization: Bearer .'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Sign in with Google or with your email.\n- type: http-bearer\n  name: Authorization\n  evidence: 'Send the key in the X-API-Key header or as Authorization: Bearer .'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in with Google or with your email.\ndocs: https://leadgen-api.adrianhomelab.com/en/start\n"
source_yaml_url: https://artifacts.apis.io/leadgen-adrianhomelab-com/authentication/leadgen-adrianhomelab-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data
- Romania
- Business
- ONRC
---
