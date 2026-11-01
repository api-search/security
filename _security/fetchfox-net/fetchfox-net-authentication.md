---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for FetchFox API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fetchfox Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: fetchfox-net declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: fetchfox-net
provider_slug: fetchfox-net
scheme_count: 2
schemes:
- evidence: Send your project key in the x-access-key header.
  header: x-access-key
  how_to_obtain: From the FetchFox dashboard or account settings.
  location: header
  name: project key
  type: apiKey
- evidence: 'Authorization: Bearer YOUR_KEY or x-access-key: YOUR_KEY.'
  header: Authorization
  how_to_obtain: From the FetchFox dashboard or account settings.
  location: header
  name: Bearer token
  type: http-bearer
slug: fetchfox-net-authentication
source_filename: fetchfox-net-authentication.yml
source_heading: Authentication Profile
source_url: https://fetchfox.net/markdown/docs
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fetchfox.net/markdown/docs\nsources:\n- https://fetchfox.net/markdown/docs\ndescription: Authentication schemes for FetchFox API\nschemes:\n- type: apiKey\n  name: project key\n  evidence: Send your project key in the x-access-key header.\n  location: header\n  header: x-access-key\n  how_to_obtain: From the FetchFox dashboard or account settings.\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Authorization: Bearer YOUR_KEY or x-access-key: YOUR_KEY.'\n  location: header\n  header: Authorization\n  how_to_obtain: From the FetchFox dashboard or account settings.\ndocs: https://fetchfox.net/markdown/docs\n"
source_yaml_url: https://artifacts.apis.io/fetchfox-net/authentication/fetchfox-net-authentication.yml
summary_line: 2 schemes
tags:
- Social Data
- API
- Media
- YouTube
- Instagram
- TikTok
---
