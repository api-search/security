---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Immunefi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Immunefi declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Immunefi
provider_slug: immunefi
scheme_count: 0
schemes: []
slug: immunefi-authentication
source_filename: immunefi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://immunefi.com/public-api/bounties.json\nnote: >-\n  Immunefi publishes no OpenAPI and no authentication documentation, so this profile was\n  established by probe rather than from a spec. The single public endpoint was fetched with no\n  credentials, no cookie and no Authorization header and returned HTTP 200 with 6,498,795 bytes of\n  application/json, so anonymous access is confirmed, not assumed. Authenticated surfaces exist\n  (the researcher application at bugs.immunefi.com and the Magnus customer console) but their\n  contracts are not public.\nsecurity_schemes:\n- name: none\n  type: none\n  in: null\n  scheme: null\n  description: >-\n    No credential of any kind is required or accepted on the public bounty-programs endpoint.\n  applies_to:\n  - GET https://immunefi.com/public-api/bounties.json\n  evidence:\n    url: https://immunefi.com/public-api/bounties.json\n    method: GET\n    request_headers_sent: [User-Agent]\n\
  \    http_status: 200\n    content_type: application/json\n    bytes: 6498795\n    fetched: '2026-08-23'\noauth2: false\nopenid_connect: false\napi_keys: false\nmutual_tls: false\ngated_surfaces:\n- name: Immunefi Bugs researcher application\n  url: https://bugs.immunefi.com/\n  status: 200\n  note: >-\n    Client-rendered application. No public API contract; account-based sign-in. Its\n    /.well-known/* paths return a Next.js 404 shell.\n- name: Immunefi support knowledge base\n  url: https://immunefisupport.zendesk.com/hc/en-us\n  status: 403\n  note: >-\n    Cloudflare interactive bot challenge (\"Enable JavaScript and cookies to continue\"), not an\n    Immunefi authorization gate. A human browser reaches the same pages; our probe was turned\n    away, so any auth detail documented there could not be read.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immunefi/refs/heads/main/authentication/immunefi-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Security
- Bug Bounty
- Vulnerability Disclosure
- Web3
- Blockchain
- Smart Contracts
- Application Security
- Cryptocurrency
- Crowdsourced Security
---
