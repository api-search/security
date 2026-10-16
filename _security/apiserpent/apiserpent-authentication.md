---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apiserpent-openapi-generated.yml
  format: yaml
  label: Contentladder Marketing API
  slug: apiserpent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiserpent/refs/heads/main/openapi/_ae-authored/apiserpent-openapi-generated.yml
auth_types: []
description: Authentication uses a Serpent API key sent in the X-API-Key header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apiserpent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Contentladder Marketing declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Contentladder Marketing
provider_slug: apiserpent
scheme_count: 1
schemes:
- evidence: You use a Serpent API key (sk_live_...) in the X-API-Key header.
  header: X-API-Key
  how_to_obtain: Create an account, then copy a sk_live_... key from the API keys page.
  location: header
  name: Serpent API Key
  type: apiKey
slug: apiserpent-authentication
source_filename: apiserpent-authentication.yml
source_heading: Authentication Profile
source_url: https://apiserpent.com/blog/google-maps-api-getting-started
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://apiserpent.com/blog/google-maps-api-getting-started\nsources:\n- https://apiserpent.com/blog/google-maps-api-getting-started\ndescription: Authentication uses a Serpent API key sent in the X-API-Key header.\nschemes:\n- type: apiKey\n  name: Serpent API Key\n  evidence: You use a Serpent API key (sk_live_...) in the X-API-Key header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an account, then copy a sk_live_... key from the API keys page.\ndocs: https://apiserpent.com/blog/google-maps-api-getting-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiserpent/refs/heads/main/authentication/apiserpent-authentication.yml
summary_line: 1 scheme
tags:
- Company
- SERP
- API
- Search
- Data
---
