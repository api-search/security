---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Activenetwork Authentication
name_suffix: Authentication
oauth_flows: []
overview: ACTIVE Network declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ACTIVE Network
provider_slug: activenetwork
scheme_count: 1
schemes:
- description: Mashery-issued developer key appended to every request as ?api_key=YOUR_KEY. Obtain by registering at https://developer.active.com/member/register.
  in: query
  name: api_key
  registration: https://developer.active.com/member/register
  type: apiKey
slug: activenetwork-authentication
source_filename: activenetwork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://developer.active.com/docs/v2_Activity_API_Search + https://developer.active.com/docs/Home\ndocs: https://developer.active.com/docs/Home\nsummary: >-\n  The public ACTIVE Network Activity Distribution APIs (Activity, Activity\n  Search v2, Campground) are read-only over public data and authenticate with a\n  Mashery-issued API key passed as an api_key query parameter. The docs state no\n  SSL/OAuth is required for the public read-only endpoints. Keys are obtained by\n  registering at the developer portal.\nschemes:\n- type: apiKey\n  name: api_key\n  in: query\n  description: >-\n    Mashery-issued developer key appended to every request as ?api_key=YOUR_KEY.\n    Obtain by registering at https://developer.active.com/member/register.\n  registration: https://developer.active.com/member/register\noauth2: false\nmutual_tls: false\nopenid_connect: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activenetwork/refs/heads/main/authentication/activenetwork-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Activities
- Events
- Recreation
- Registration
- Endurance
- Campgrounds
- Sports
- Search
---
