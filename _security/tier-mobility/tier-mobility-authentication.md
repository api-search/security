---
anonymous_access: true
api_key_in: []
api_specs:
- filename: tier-mobility-discovery-api-openapi.yml
  format: yaml
  label: TIER Discovery API
  slug: tier-mobility-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/openapi/tier-mobility-discovery-api-openapi.yml
- filename: tier-mobility-stations-api-openapi.yml
  format: yaml
  label: TIER Stations API
  slug: tier-mobility-stations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/openapi/tier-mobility-stations-api-openapi.yml
- filename: tier-mobility-system-api-openapi.yml
  format: yaml
  label: TIER System API
  slug: tier-mobility-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/openapi/tier-mobility-system-api-openapi.yml
- filename: tier-mobility-vehicles-api-openapi.yml
  format: yaml
  label: TIER Vehicles API
  slug: tier-mobility-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/openapi/tier-mobility-vehicles-api-openapi.yml
- filename: tier-mobility-zones-api-openapi.yml
  format: yaml
  label: TIER Zones API
  slug: tier-mobility-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/openapi/tier-mobility-zones-api-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tier Mobility Authentication
name_suffix: Authentication
oauth_flows: []
overview: TIER secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TIER
provider_slug: tier-mobility
scheme_count: 2
schemes:
- applies_to: https://gbfs.api.ridedott.com/public/v2/
  description: Public GBFS 2.3 discovery and data feeds need no credential.
  evidence:
  - status: 200
    url: https://gbfs.api.ridedott.com/public/v2/berlin/gbfs.json
  - status: 200
    url: https://gbfs.api.ridedott.com/public/v2/gbfs_versions.json
  name: publicGbfs
  type: none
- applies_to: https://gbfs.api.ridedott.com (non-public paths — Dott Partner API)
  description: 'Per-partner API Key issued by Dott. The licence states: "You must obtain a security key ("API Key") through a registration process communicated by Dott", the key may not be shared or embedded in open source, must be the sole means of access, and may be revoked at any time.'
  evidence:
  - finding: licence text requires a Dott-issued API Key
    status: 200
    url: https://ridedott.com/api-licence/
  - finding: 'no header -> {"error":"Unauthorized: missing authorization header"}'
    status: 401
    url: https://gbfs.api.ridedott.com/
  - finding: 'Authorization: Bearer <invalid> -> {"error":"Forbidden: access denied"} (scheme accepted, key refused)'
    status: 403
    url: https://gbfs.api.ridedott.com/
  - finding: 'Authorization without a Bearer/with Basic -> {"error":"Unauthorized: invalid authorization header"}'
    status: 401
    url: https://gbfs.api.ridedott.com/
  header: Authorization
  in: header
  issuance: Registration process communicated by Dott (no self-serve signup is published).
  name: partnerApiKey
  revocable: true
  scheme: bearer
  type: http
slug: tier-mobility-authentication
source_filename: tier-mobility-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: searched\nsource: https://ridedott.com/api-licence/\ndocs: https://ridedott.com/api-licence/\nnote: >-\n  The refined GBFS OpenAPIs declare no securitySchemes (derive-authentication.py found none) because\n  the public GBFS 2.3 feeds under https://gbfs.api.ridedott.com/public/v2/ answer anonymously. The\n  partner surface on the same host is key-gated: Dott's API Licence requires an API Key obtained\n  through a registration process Dott communicates to the licensee, and the host rejects requests\n  without an Authorization header. The header scheme below was established by live probing, not\n  from published docs — Dott does not publish a partner auth reference.\nsummary:\n  types:\n  - none\n  - http\n  api_key_locations:\n  - header\nschemes:\n- name: publicGbfs\n  type: none\n  applies_to: https://gbfs.api.ridedott.com/public/v2/\n  description: Public GBFS 2.3 discovery and data feeds need no credential.\n  evidence:\n  - url: https://gbfs.api.ridedott.com/public/v2/berlin/gbfs.json\n\
  \    status: 200\n  - url: https://gbfs.api.ridedott.com/public/v2/gbfs_versions.json\n    status: 200\n- name: partnerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  applies_to: https://gbfs.api.ridedott.com (non-public paths — Dott Partner API)\n  description: >-\n    Per-partner API Key issued by Dott. The licence states: \"You must obtain a security key\n    (\"API Key\") through a registration process communicated by Dott\", the key may not be shared\n    or embedded in open source, must be the sole means of access, and may be revoked at any time.\n  issuance: Registration process communicated by Dott (no self-serve signup is published).\n  revocable: true\n  evidence:\n  - url: https://ridedott.com/api-licence/\n    status: 200\n    finding: licence text requires a Dott-issued API Key\n  - url: https://gbfs.api.ridedott.com/\n    status: 401\n    finding: 'no header -> {\"error\":\"Unauthorized: missing authorization header\"}'\n  - url: https://gbfs.api.ridedott.com/\n\
  \    status: 403\n    finding: 'Authorization: Bearer <invalid> -> {\"error\":\"Forbidden: access denied\"} (scheme accepted, key refused)'\n  - url: https://gbfs.api.ridedott.com/\n    status: 401\n    finding: 'Authorization without a Bearer/with Basic -> {\"error\":\"Unauthorized: invalid authorization header\"}'\nrelated:\n  wordpress_mcp_oauth:\n    note: >-\n      Separate from the data API: ridedott.com (the WordPress corporate site) publishes OAuth 2.0\n      authorization-server and protected-resource metadata for the WordPress MCP Adapter endpoint\n      https://ridedott.com/wp-json/mcp/mcp-oauth-server (authorization_code + PKCE S256, public\n      clients, scope \"mcp\"). tools/list returns 401 mcp_unauthorized. This is a platform-authored CMS\n      surface, not documented by Dott as a developer product; see well-known/.\n    authorization_endpoint: https://ridedott.com/oauth/authorize\n    token_endpoint: https://ridedott.com/oauth/token\n    scopes:\n    - mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tier-mobility/refs/heads/main/authentication/tier-mobility-authentication.yml
summary_line: none/http · 2 schemes
tags:
- Mobility
- Micromobility
- Shared Mobility
- E-Scooter
- E-Bikes
- Transportation
- Smart Cities
- MaaS
- GBFS
- Open Data
- Europe
- Real-Time
---
