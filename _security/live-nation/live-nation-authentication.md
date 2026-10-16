---
anonymous_access: false
api_key_in: []
api_specs:
- filename: live-nation-openapi-generated.yml
  format: yaml
  label: Live Nation API
  slug: live-nation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/live-nation/refs/heads/main/openapi/_ae-authored/live-nation-openapi-generated.yml
auth_types: []
description: Ticketmaster APIs use an API key passed as a query parameter.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Live Nation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Live Nation declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Live Nation
provider_slug: live-nation
scheme_count: 1
schemes:
- evidence: 'All API calls follow this format: https://app.ticketmaster.com/{package}/{version}/{resource}.json?apikey=**{API key}'
  how_to_obtain: Register for an API key on the Ticketmaster Developer Portal.
  location: query
  name: apikey
  type: apiKey
slug: live-nation-authentication
source_filename: live-nation-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.ticketmaster.com/products-and-docs/apis/getting-started/
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.ticketmaster.com/products-and-docs/apis/getting-started/\nsources:\n- https://developer.ticketmaster.com/products-and-docs/apis/getting-started/\n- https://developer.ticketmaster.com/products-and-docs/apis/getting-started/\ndescription: Ticketmaster APIs use an API key passed as a query parameter.\nschemes:\n- type: apiKey\n  name: apikey\n  evidence: 'All API calls follow this format: https://app.ticketmaster.com/{package}/{version}/{resource}.json?apikey=**{API key}'\n  location: query\n  how_to_obtain: Register for an API key on the Ticketmaster Developer Portal.\ndocs: https://developer.ticketmaster.com/products-and-docs/apis/getting-started/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/live-nation/refs/heads/main/authentication/live-nation-authentication.yml
summary_line: 1 scheme
tags:
- Entertainment
- Ticketing
- Live Events
- Music
- Technology
---
