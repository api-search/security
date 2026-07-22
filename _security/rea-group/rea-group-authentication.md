---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Rea Group Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: REA Group secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: REA Group
provider_slug: rea-group
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    note: token endpoint issued to partners during onboarding; not public
    tokenUrl: null
  name: OAuth2
  sources:
  - https://developer.proptrack.com.au/docs/apis/authentication
  type: oauth2
slug: rea-group-authentication
source_filename: rea-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.proptrack.com.au/docs/apis/authentication\ndocs: https://developer.proptrack.com.au/docs/apis/authentication\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  notes: >-\n    PropTrack (REA Group) APIs are protected by OAuth 2.0 (the auth docs page is\n    titled \"OAuth 2.0 | PropTrack APIs\"). Access is partner-gated: a client is\n    issued credentials under a commercial agreement and exchanges them with the\n    REA Group OAuth identity service for a bearer access token used against\n    data.proptrack.com. The specific token endpoint URL and scope list are not\n    published on the public developer surface (partner onboarding material).\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: null\n    note: token endpoint issued to partners during onboarding; not public\n  sources: [https://developer.proptrack.com.au/docs/apis/authentication]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/authentication/rea-group-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Real Estate
- Property Data
- Valuations
- Market Insights
- Listings
- PropTech
- Australia
---
