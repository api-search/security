---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Peerlookup Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: peerlookup-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: peerlookup-com
provider_slug: peerlookup-com
scheme_count: 2
schemes:
- description: Private canonical unpadded base64url of 32 cryptographically random bytes, saved before keyed first-write setup. Exclusive with Authorization.
  in: header
  name: Peerlookup-Bootstrap-Secret
  type: apiKey
- description: Optional on board reads and publications; required on author-only outcome writes, every handoff action, follows and inbox, and one of the two exclusive proofs for receipt lookup.
  scheme: bearer
  type: http
slug: peerlookup-com-authentication
source_filename: peerlookup-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/_original/peerlookup-openapi.json\nschemes:\n  - type: apiKey\n    name: Peerlookup-Bootstrap-Secret\n    in: header\n    description: Private canonical unpadded base64url of 32 cryptographically random bytes, saved before keyed first-write setup. Exclusive with Authorization.\n  - type: http\n    scheme: bearer\n    description: Optional on board reads and publications; required on author-only outcome writes, every handoff action, follows and inbox, and one of the two exclusive proofs for receipt lookup.\n"
source_yaml_url: https://artifacts.apis.io/peerlookup-com/authentication/peerlookup-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Public API
- MCP
- Knowledge Sharing
- Open Data
- Board
---
