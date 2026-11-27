---
anonymous_access: false
api_key_in: []
api_specs:
- filename: onyphe-asd-api-openapi.yml
  format: yaml
  label: ONYPHE ASD API
  slug: onyphe-asd-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onyphe/openapi/onyphe-asd-api-openapi.yml
- filename: onyphe-discovery-api-openapi.yml
  format: yaml
  label: ONYPHE Discovery API
  slug: onyphe-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onyphe/openapi/onyphe-discovery-api-openapi.yml
- filename: onyphe-export-api-openapi.yml
  format: yaml
  label: ONYPHE Export API
  slug: onyphe-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onyphe/openapi/onyphe-export-api-openapi.yml
- filename: onyphe-search-api-openapi.yml
  format: yaml
  label: ONYPHE Search API
  slug: onyphe-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onyphe/openapi/onyphe-search-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ONYPHE Authentication
name_suffix: Authentication
oauth_flows: []
overview: ONYPHE declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ONYPHE
provider_slug: onyphe
scheme_count: 1
schemes:
- evidence: 'curl -H ''Content-Type: application/json'' -H ''Authorization: bearer YOUR_APIKEY'' -XGET ''https://www.onyphe.io/api/v2/search/?q=protocol:rdp'''
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: onyphe-authentication
source_filename: onyphe-authentication.yml
source_heading: Authentication Profile
source_url: https://search.onyphe.io/docs/getting-started
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://search.onyphe.io/docs/getting-started\nsources:\n- https://search.onyphe.io/docs/getting-started\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl -H ''Content-Type: application/json'' -H ''Authorization: bearer YOUR_APIKEY'' -XGET ''https://www.onyphe.io/api/v2/search/?q=protocol:rdp'''\n  location: header\n  header: Authorization\ndocs: https://search.onyphe.io/docs/getting-started\n"
source_yaml_url: https://artifacts.apis.io/onyphe/authentication/onyphe-authentication.yml
summary_line: 1 scheme
tags:
- Attack Surface Management
- Threat Intelligence
- Internet Scanning
- Passive DNS
- Vulnerability Data
---
