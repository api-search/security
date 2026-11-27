---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for RealtyCrawl as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: RealtyCrawl Authentication
name_suffix: Authentication
oauth_flows: []
overview: RealtyCrawl declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: RealtyCrawl
provider_slug: realtycrawl
scheme_count: 2
schemes:
- evidence: 'Send one Authorization: Bearer header with a live rc_live_ key.'
  header: Authorization
  how_to_obtain: Create and copy a live API key in the dashboard; the key value is used as the bearer token.
  location: header
  name: Bearer
  type: http-bearer
- evidence: X-API-Key is supported as an alternative; do not send both.
  header: X-API-Key
  how_to_obtain: Create and copy a live API key in the dashboard; the key value is sent in the X-API-Key header.
  location: header
  name: X-API-Key
  type: apiKey
slug: realtycrawl-authentication
source_filename: realtycrawl-authentication.yml
source_heading: Authentication Profile
source_url: https://realtycrawl.dev/docs/authentication
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://realtycrawl.dev/docs/authentication\nsources:\n- https://realtycrawl.dev/docs/authentication\n- https://realtycrawl.dev/docs/quickstart\n- https://realtycrawl.dev/docs\n- https://realtycrawl.dev/docs/agent-skills\ndescription: Authentication schemes for RealtyCrawl as documented.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send one Authorization: Bearer header with a live rc_live_ key.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create and copy a live API key in the dashboard; the key value is used as the bearer token.\n- type: apiKey\n  name: X-API-Key\n  evidence: X-API-Key is supported as an alternative; do not send both.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create and copy a live API key in the dashboard; the key value is sent in the X-API-Key header.\ndocs: https://realtycrawl.dev/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/realtycrawl/authentication/realtycrawl-authentication.yml
summary_line: 2 schemes
tags:
- Real Estate
- Data
- Listings
- Aggregation
- Company
---
