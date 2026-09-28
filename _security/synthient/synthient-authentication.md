---
anonymous_access: false
api_key_in: []
api_specs:
- filename: synthient-account-api-openapi.yml
  format: yaml
  label: Synthient API Account API
  slug: synthient-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-account-api-openapi.yml
- filename: synthient-anonymizers-api-openapi.yml
  format: yaml
  label: Synthient API Anonymizers API
  slug: synthient-anonymizers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-anonymizers-api-openapi.yml
- filename: synthient-helios-api-openapi.yml
  format: yaml
  label: Synthient API Helios API
  slug: synthient-helios-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-helios-api-openapi.yml
- filename: synthient-ja4t-api-openapi.yml
  format: yaml
  label: Synthient API JA4T API
  slug: synthient-ja4t-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-ja4t-api-openapi.yml
- filename: synthient-lookup-api-openapi.yml
  format: yaml
  label: Synthient API Lookup API
  slug: synthient-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-lookup-api-openapi.yml
- filename: synthient-proxies-api-openapi.yml
  format: yaml
  label: Synthient API Proxies API
  slug: synthient-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-proxies-api-openapi.yml
- filename: synthient-torrents-api-openapi.yml
  format: yaml
  label: Synthient API Torrents API
  slug: synthient-torrents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/openapi/synthient-torrents-api-openapi.yml
auth_types: []
description: Authentication schemes for Synthient API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Synthient Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synthient API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Synthient API
provider_slug: synthient
scheme_count: 1
schemes:
- evidence: Every request to Synthient is authenticated with a single API key, which carries a set of scopes that determine which endpoints and feeds you can access.
  header: x-api-key
  how_to_obtain: API keys are issued from the Synthient dashboard. If you don't have one yet, contact us and we'll provision one with the scopes you need.
  location: header
  name: API Key
  type: apiKey
slug: synthient-authentication
source_filename: synthient-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.synthient.com/authentication
source_yaml: "generated: '2026-09-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.synthient.com/authentication\nsources:\n- https://docs.synthient.com/authentication\ndescription: Authentication schemes for Synthient API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Every request to Synthient is authenticated with a single API key, which carries a set of scopes that determine which endpoints and\n    feeds you can access.\n  location: header\n  header: x-api-key\n  how_to_obtain: API keys are issued from the Synthient dashboard. If you don't have one yet, contact us and we'll provision one with the scopes\n    you need.\nnote: No OAuth2 or other authentication schemes are documented on the page.\ndocs: https://docs.synthient.com/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synthient/refs/heads/main/authentication/synthient-authentication.yml
summary_line: 1 scheme
tags:
- Company
- IP
- Enrichment
- Cybersecurity
- Data
---
