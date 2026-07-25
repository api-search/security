---
api_key_in: []
api_specs:
- filename: blockchalk-chalks-api-openapi.yml
  format: yaml
  label: BlockChalk chalks API
  slug: blockchalk-chalks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchalk/refs/heads/main/openapi/blockchalk-chalks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Blockchalk Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlockChalk declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: BlockChalk
provider_slug: blockchalk
scheme_count: 0
schemes: []
slug: blockchalk-authentication
source_filename: blockchalk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: http://web.archive.org/web/20090810213933/http://blockchalk.com/developers\ndocs: http://web.archive.org/web/20090810213933/http://blockchalk.com/developers\nname: BlockChalk authentication profile\nstatus: retired\nsummary: >-\n  BlockChalk's published API surface was fully anonymous. The developer page documented three\n  read interfaces (XML, JSON, RSS) parameterized only by latitude and longitude, with no\n  API key, token, signature or registration step of any kind. Captured live responses from\n  /api/v0.6/chalks confirm unauthenticated public reads.\nschemes: []\nsecurity_requirements:\n  global: none\n  notes: >-\n    OpenAPI security is an empty array in openapi/blockchalk-chalks-openapi.yml, reflecting\n    the documented anonymous access model.\nregistration:\n  required: false\n  developer_signup: false\n  key_provisioning: none\noauth2: false\nopenid_connect: false\nmutual_tls: false\nwrite_access:\n  published:\
  \ false\n  notes: >-\n    Only read interfaces were ever published. Posting a chalk was done through the BlockChalk\n    mobile clients, and no public write API or credential model was documented.\ncaveats:\n  - The service is retired; this profile is historical and not actionable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockchalk/refs/heads/main/authentication/blockchalk-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Location
- Geolocation
- Social
- Messaging
- Local
- Neighborhood
- Mobile
- Retired
---
