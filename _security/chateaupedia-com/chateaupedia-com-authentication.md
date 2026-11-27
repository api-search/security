---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chateaupedia-com-openapi-generated.yml
  format: yaml
  label: Chateaupedia API
  slug: chateaupedia-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chateaupedia-com/openapi/_ae-authored/chateaupedia-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Chateaupedia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chateaupedia declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Chateaupedia
provider_slug: chateaupedia-com
scheme_count: 2
schemes:
- description: 'The key goes in the Authorization header. Example from the docs: curl -H "Authorization: Bearer ck_live_…" https://chateaupedia.com/api/dataset.json?limit=100'
  in: header
  key_prefix: ck_live_
  name: Authorization
  scheme: bearer
  type: http
- description: 'A ?key= parameter is accepted for tools that cannot send headers, but it ends up in proxy logs: prefer the header.'
  in: query
  name: key
  type: apiKey
slug: chateaupedia-com-authentication
source_filename: chateaupedia-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://chateaupedia.com/en/api\ndocs: https://chateaupedia.com/en/api\nschemes:\n- type: http\n  scheme: bearer\n  name: Authorization\n  in: header\n  key_prefix: ck_live_\n  description: 'The key goes in the Authorization header. Example from the docs: curl -H \"Authorization: Bearer ck_live_…\" https://chateaupedia.com/api/dataset.json?limit=100'\n- type: apiKey\n  name: key\n  in: query\n  description: 'A ?key= parameter is accepted for tools that cannot send headers, but it ends up in proxy logs: prefer the header.'\nkey_issuance: 'Keys are issued by hand for now: we read every request. Allow 48 working hours. The key is free.'\nunauthenticated_surfaces:\n- GET /en/castle/{slug}.md (Markdown version of every entry, no key needed)\n- GET /llms.txt (no key needed)\n- https://chateaupedia.com/opendata/chateaux.csv (no key, per llms.txt)\n"
source_yaml_url: https://artifacts.apis.io/chateaupedia-com/authentication/chateaupedia-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Castles
- Tourism
- Travel
- Cultural Heritage
- Open Data
- Directory
- France
- Germany
---
