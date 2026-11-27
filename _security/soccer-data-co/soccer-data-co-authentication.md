---
anonymous_access: false
api_key_in: []
api_specs:
- filename: soccer-data-co-openapi-generated.yml
  format: yaml
  label: Soccer Data API
  slug: soccer-data-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soccer-data-co/openapi/_ae-authored/soccer-data-co-openapi-generated.yml
auth_types: []
description: Authentication methods for Soccer Data API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Soccer Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soccer Data declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Soccer Data
provider_slug: soccer-data-co
scheme_count: 2
schemes:
- evidence: 'Put the key in the X-Api-Key header:'
  header: X-Api-Key
  how_to_obtain: Your first key is created automatically when you sign up; additional keys can be created on the API keys page of your dashboard.
  location: header
  name: API Key
  type: apiKey
- evidence: 'If your HTTP client is already set up for bearer tokens, Authorization: Bearer YOUR_API_KEY works too.'
  header: Authorization
  how_to_obtain: Your first key is created automatically when you sign up; additional keys can be created on the API keys page of your dashboard.
  location: header
  name: Bearer Token
  type: http-bearer
slug: soccer-data-co-authentication
source_filename: soccer-data-co-authentication.yml
source_heading: Authentication Profile
source_url: https://soccer-data.co/docs/authentication
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://soccer-data.co/docs/authentication\nsources:\n- https://soccer-data.co/docs/authentication\n- https://soccer-data.co/docs/quickstart\ndescription: Authentication methods for Soccer Data API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Put the key in the X-Api-Key header:'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Your first key is created automatically when you sign up; additional keys can be created on the API keys page of your dashboard.\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'If your HTTP client is already set up for bearer tokens, Authorization: Bearer YOUR_API_KEY works too.'\n  location: header\n  header: Authorization\n  how_to_obtain: Your first key is created automatically when you sign up; additional keys can be created on the API keys page of your dashboard.\ndocs: https://soccer-data.co/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/soccer-data-co/authentication/soccer-data-co-authentication.yml
summary_line: 2 schemes
tags:
- Football API
- Live Scores
- Odds
- Betting
- Fantasy Games
---
