---
anonymous_access: false
api_key_in: []
api_specs:
- filename: checkmails-eu-bulk-api-openapi.yml
  format: yaml
  label: checkmails Bulk API
  slug: checkmails-eu-bulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkmails-eu/openapi/checkmails-eu-bulk-api-openapi.yml
- filename: checkmails-eu-jobs-api-openapi.yml
  format: yaml
  label: checkmails Jobs API
  slug: checkmails-eu-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkmails-eu/openapi/checkmails-eu-jobs-api-openapi.yml
- filename: checkmails-eu-verify-api-openapi.yml
  format: yaml
  label: checkmails Verify API
  slug: checkmails-eu-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/checkmails-eu/openapi/checkmails-eu-verify-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: checkmails Authentication
name_suffix: Authentication
oauth_flows: []
overview: checkmails secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: checkmails
provider_slug: checkmails-eu
scheme_count: 1
schemes:
- applies_to:
  - REST API (https://checkmails.eu/api/v1/*)
  - MCP server (https://checkmails.eu/api/mcp), same Authorization Bearer chk_<key> header
  bearerFormat: chk_<32hex>
  description: Keys start with chk_ followed by 32 hexadecimal characters. Generated from the dashboard (Profile tab → API Keys section); shown only once at creation time. REST API access requires a paid plan.
  header: 'Authorization: Bearer chk_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/checkmails-eu-openapi.yml
  - https://checkmails.eu/docs
  type: http
slug: checkmails-eu-authentication
source_filename: checkmails-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://checkmails.eu/docs\ndocs: https://checkmails.eu/docs\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: chk_<32hex>\n  header: 'Authorization: Bearer chk_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'\n  description: Keys start with chk_ followed by 32 hexadecimal characters. Generated from the dashboard (Profile tab → API Keys section); shown only once at creation time. REST API access requires a paid plan.\n  applies_to:\n  - REST API (https://checkmails.eu/api/v1/*)\n  - MCP server (https://checkmails.eu/api/mcp), same Authorization Bearer chk_<key> header\n  sources:\n  - openapi/checkmails-eu-openapi.yml\n  - https://checkmails.eu/docs\nkey_errors:\n- {status: 401, code: missing_bearer, meaning: Missing Authorization header}\n- {status: 401, code: invalid_key_format, meaning: Key does not start with chk_ or is too short}\n- {status: 401, code: invalid_key, meaning: Key\
  \ not found}\n- {status: 401, code: revoked_key, meaning: Key has been revoked}\n"
source_yaml_url: https://artifacts.apis.io/checkmails-eu/authentication/checkmails-eu-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Email Verification
- SMTP
- GDPR
- Data Quality
- European Union
- MCP
- Odoo
---
