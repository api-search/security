---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mygeocode-openapi-generated.yml
  format: yaml
  label: My Geocode API
  slug: mygeocode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mygeocode/openapi/_ae-authored/mygeocode-openapi-generated.yml
auth_types: []
description: 'Authentication: API keys, credit and IP slots'
kind: authentication
layout: security
mechanism_count: 8
method: searched
name: My Geocode Authentication
name_suffix: Authentication
oauth_flows: []
overview: My Geocode declares 8 security scheme(s) across its OpenAPI definitions.
provider_name: My Geocode
provider_slug: mygeocode
scheme_count: 8
schemes:
- evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'
  location: query
  name: key (query)
  type: apiKey
- evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'
  header: Authorization
  location: header
  name: Basic
  type: http-basic
- evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'
  header: X-Goog-Api-Key
  location: header
  name: X-Goog-Api-Key
  type: other
- evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'
  header: X-API-Token
  location: header
  name: X-API-Token
  type: other
- evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'
  header: X-Access-Token
  location: header
  name: X-Access-Token
  type: other
- evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'
  location: body
  name: form body
  type: other
slug: mygeocode-authentication
source_filename: mygeocode-authentication.yml
source_heading: Authentication Profile
source_url: https://www.mygeocode.com/docs/authentication/
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.mygeocode.com/docs/authentication/\nsources:\n- https://www.mygeocode.com/docs/authentication/\n- https://www.mygeocode.com/es/docs/authentication/\n- https://www.mygeocode.com/fr/docs/authentication/\n- https://www.mygeocode.com/pt/docs/authentication/\ndescription: 'Authentication: API keys, credit and IP slots'\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'\n  location: header\n  header: X-API-Key\n- type: http-bearer\n  name: Authorization\n  evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: key (query)\n  evidence: 'Any of these works on every host. Prefer the header: query strings\
  \ end up in server logs, browser histories and proxies.'\n  location: query\n- type: http-basic\n  name: Basic\n  evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'\n  location: header\n  header: Authorization\n- type: other\n  name: X-Goog-Api-Key\n  evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'\n  location: header\n  header: X-Goog-Api-Key\n- type: other\n  name: X-API-Token\n  evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'\n  location: header\n  header: X-API-Token\n- type: other\n  name: X-Access-Token\n  evidence: 'Any of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'\n  location: header\n  header: X-Access-Token\n- type: other\n  name: form body\n  evidence: 'Any\
  \ of these works on every host. Prefer the header: query strings end up in server logs, browser histories and proxies.'\n  location: body\nnote: OAuth2 flows are not described on the pages.\ndocs: https://www.mygeocode.com/docs/authentication/\n"
source_yaml_url: https://artifacts.apis.io/mygeocode/authentication/mygeocode-authentication.yml
summary_line: 8 schemes
tags:
- Geocoding
- IP Lookup
- Timezone
- Elevation
- Postal Code
---
