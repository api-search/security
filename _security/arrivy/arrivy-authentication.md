---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arrivy-entity-apis-api-openapi.yml
  format: yaml
  label: Arrivy Entity APIs API
  slug: arrivy-entity-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arrivy/openapi/arrivy-entity-apis-api-openapi.yml
- filename: arrivy-location-report-apis-api-openapi.yml
  format: yaml
  label: Arrivy Location Report APIs API
  slug: arrivy-location-report-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arrivy/openapi/arrivy-location-report-apis-api-openapi.yml
- filename: arrivy-task-apis-api-openapi.yml
  format: yaml
  label: Arrivy Task APIs API
  slug: arrivy-task-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arrivy/openapi/arrivy-task-apis-api-openapi.yml
- filename: arrivy-task-status-apis-api-openapi.yml
  format: yaml
  label: Arrivy Task Status APIs API
  slug: arrivy-task-status-apis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arrivy/openapi/arrivy-task-status-apis-api-openapi.yml
auth_types: []
description: Arrivy uses two custom header keys for authentication.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Arrivy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arrivy declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Arrivy
provider_slug: arrivy
scheme_count: 2
schemes:
- evidence: 'Once you signup and login to your Arrivy account you can find two auth keys on your API page. To authenticate with our APIs you will need to set these two custom headers: X-Auth-Key and X-Auth-Token in each API call.'
  header: X-Auth-Key
  how_to_obtain: You can request a new pair of keys via the web portal by going to API tab and clicking "Request New Keys".
  location: header
  name: X-Auth-Key
  type: apiKey
- evidence: 'Once you signup and login to your Arrivy account you can find two auth keys on your API page. To authenticate with our APIs you will need to set these two custom headers: X-Auth-Key and X-Auth-Token in each API call.'
  header: X-Auth-Token
  how_to_obtain: You can request a new pair of keys via the web portal by going to API tab and clicking "Request New Keys".
  location: header
  name: X-Auth-Token
  type: apiKey
slug: arrivy-authentication
source_filename: arrivy-authentication.yml
source_heading: Authentication Profile
source_url: https://app.arrivy.com/developer-portal/building-blocks#authentication-scheme-1
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.arrivy.com/developer-portal/building-blocks#authentication-scheme-1\nsources:\n- https://app.arrivy.com/developer-portal/building-blocks#authentication-scheme-1\n- https://app.arrivy.com/developer-portal/building-blocks#getting-started-1\ndescription: Arrivy uses two custom header keys for authentication.\nschemes:\n- type: apiKey\n  name: X-Auth-Key\n  evidence: 'Once you signup and login to your Arrivy account you can find two auth keys on your API page. To authenticate with our APIs you will\n    need to set these two custom headers: X-Auth-Key and X-Auth-Token in each API call.'\n  location: header\n  header: X-Auth-Key\n  how_to_obtain: You can request a new pair of keys via the web portal by going to API tab and clicking \"Request New Keys\".\n- type: apiKey\n  name: X-Auth-Token\n  evidence: 'Once you signup and login to your Arrivy account you can find two auth\
  \ keys on your API page. To authenticate with our APIs you will\n    need to set these two custom headers: X-Auth-Key and X-Auth-Token in each API call.'\n  location: header\n  header: X-Auth-Token\n  how_to_obtain: You can request a new pair of keys via the web portal by going to API tab and clicking \"Request New Keys\".\ndocs: https://app.arrivy.com/developer-portal/building-blocks#authentication-scheme-1\n"
source_yaml_url: https://artifacts.apis.io/arrivy/authentication/arrivy-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Field Service Management
- Operations Software
- Cloud Platform
- Integration
---
