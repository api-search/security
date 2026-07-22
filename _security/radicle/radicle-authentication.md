---
api_key_in: []
api_specs:
- filename: radicle-httpd-openapi.yml
  format: yaml
  label: Radicle HTTP API
  slug: radicle-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radicle/refs/heads/main/openapi/radicle-httpd-openapi.yml
auth_types:
- none
- session
description: ''
kind: authentication
layout: security
method: searched
name: Radicle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Radicle secures its APIs with none and session across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Radicle
provider_slug: radicle
scheme_count: 2
schemes:
- applies_to: All GET endpoints on a public seed node
  name: publicRead
  sources:
  - openapi/radicle-httpd-openapi.yml
  - live probe of seed.radicle.xyz
  type: none
- description: 'Write-capable radicle-httpd deployments authenticate a session with the node operator''s key: a client requests a session, then authorizes it by signing a challenge with the Radicle key (via the desktop app / CLI). Public community seeds (e.g. seed.radicle.xyz) expose read endpoints only, so no session is required for the surface captured here.'
  name: nodeSession
  sources:
  - radicle-httpd
  type: session
slug: radicle-authentication
source_filename: radicle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://seed.radicle.xyz/api/v1 (live probe) + radicle-httpd behavior\ndocs: https://radicle.dev/guides\nsummary:\n  types: [none, session]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    Radicle uses no accounts, passwords or OAuth. Identity is cryptographic:\n    every peer is a DID (did:key, e.g. z6Mk...). The radicle-httpd JSON API is\n    read-only and unauthenticated for all catalog/read endpoints exposed by a\n    public seed node (repos, issues, patches, commits, trees, node, stats).\nschemes:\n- name: publicRead\n  type: none\n  applies_to: All GET endpoints on a public seed node\n  sources: [openapi/radicle-httpd-openapi.yml, live probe of seed.radicle.xyz]\n- name: nodeSession\n  type: session\n  description: >-\n    Write-capable radicle-httpd deployments authenticate a session with the\n    node operator's key: a client requests a session, then authorizes it by\n    signing a challenge with the Radicle\
  \ key (via the desktop app / CLI). Public\n    community seeds (e.g. seed.radicle.xyz) expose read endpoints only, so no\n    session is required for the surface captured here.\n  sources: [radicle-httpd]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radicle/refs/heads/main/authentication/radicle-authentication.yml
summary_line: none/session · 2 schemes
tags:
- Company
- Developer Tools
- Code Collaboration
- Git
- Peer-to-Peer
- Version Control
- Open Source
- Decentralized
- Developer Tools API
---
