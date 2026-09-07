---
api_specs:
- filename: anew-openapi.json
  format: json
  label: anew Write/Read API
  slug: anew-writeread-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anew/refs/heads/main/openapi/anew-openapi.json
certification_count: 0
certifications: []
description: ''
kind: trust-center
layout: security
name: Anew Trust Center
name_suffix: Trust Center
overview: anew maintains a public trust center covering its security and compliance posture.
provider_name: anew
provider_slug: anew
slug: anew-trust-center
source_filename: anew-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://anew.page/llms.txt + https://github.com/round/anew.page/blob/main/LICENSE.md + probes of trust/status/compliance paths\npublished: false\nsummary: >-\n  No trust center, no certifications, and no compliance program. What anew publishes instead is a\n  structural privacy argument: there is no account, no cookie and no profile, a page travels inside its\n  own URL rather than being stored, and nothing is retained — so there is, as the policy puts it,\n  \"nothing you would ever need to access or delete\".\ntrust_center_url: null\ncertifications: []\nsubprocessors_published: false\nprivacy_policy: https://github.com/round/anew.page/blob/main/LICENSE.md\nterms_of_service: https://github.com/round/anew.page/blob/main/LICENSE.md\ndata_retention:\n  model: none\n  detail: >-\n    No source HTML and no page record are kept — the URL carries the page. The single exception the\n    provider documents is a best-effort screenshot\
  \ render cached publicly at the page's .png twin.\n  caveat: >-\n    A consequence worth stating plainly for buyers: because the page rides in the URL, anyone with the\n    URL can decode it. The provider says so directly — anew is explicitly not for content that must stay\n    private.\nabuse_controls:\n  - control: threat-feed link blocking\n    detail: >-\n      A page whose outbound links reach a host currently flagged by Cloudflare's or Google's threat feeds\n      is refused with 451 content_blocked before it renders.\n  - control: rate limiting\n    detail: 300 requests per 60 seconds per client IP across /write, /mcp and /a2a/v1.\n  - control: script handling\n    detail: >-\n      The MCP tool contract rejects script elements and inline event handlers inside `html`, requiring\n      JavaScript to be passed separately so the server controls where it is inserted.\nprobed:\n  - url: https://anew.page/status\n    status: 404\n  - url: https://anew.page/terms\n    status: 404\n  -\
  \ url: https://anew.page/privacy\n    status: 404\nnote: >-\n  Recorded as an affirmative absence. For a free, accountless, zero-retention utility this is a\n  defensible posture rather than a gap, but a buyer with a vendor-review checklist will find nothing to\n  put in it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anew/refs/heads/main/security/anew-trust-center.yml
summary_line: trust center published
tags:
- html
- webpage
- website
- url
- encode
- share
- web-publishing
- developer-tools
- mcp
- a2a
- ai-agent-tooling
- llms-txt
- agents-txt
- agent-skills
- webmcp
- openapi
- stateless
- immutable
- no-auth
- static-site
- url-encoding
trust_url: ''
---
