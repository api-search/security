---
api_key_in:
- header
api_specs:
- filename: podcastindex-add-api-openapi.yml
  format: yaml
  label: PodcastIndex Add API
  slug: podcastindex-add-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-add-api-openapi.yml
- filename: podcastindex-apple-replacement-api-openapi.yml
  format: yaml
  label: PodcastIndex Apple Replacement API
  slug: podcastindex-apple-replacement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-apple-replacement-api-openapi.yml
- filename: podcastindex-categories-api-openapi.yml
  format: yaml
  label: PodcastIndex Categories API
  slug: podcastindex-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-categories-api-openapi.yml
- filename: podcastindex-episodes-api-openapi.yml
  format: yaml
  label: PodcastIndex Episodes API
  slug: podcastindex-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-episodes-api-openapi.yml
- filename: podcastindex-hub-api-openapi.yml
  format: yaml
  label: PodcastIndex Hub API
  slug: podcastindex-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-hub-api-openapi.yml
- filename: podcastindex-podcasts-api-openapi.yml
  format: yaml
  label: PodcastIndex Podcasts API
  slug: podcastindex-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-podcasts-api-openapi.yml
- filename: podcastindex-recent-api-openapi.yml
  format: yaml
  label: PodcastIndex Recent API
  slug: podcastindex-recent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-recent-api-openapi.yml
- filename: podcastindex-search-api-openapi.yml
  format: yaml
  label: PodcastIndex Search API
  slug: podcastindex-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-search-api-openapi.yml
- filename: podcastindex-static-data-api-openapi.yml
  format: yaml
  label: PodcastIndex Static Data API
  slug: podcastindex-static-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-static-data-api-openapi.yml
- filename: podcastindex-stats-api-openapi.yml
  format: yaml
  label: PodcastIndex Stats API
  slug: podcastindex-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-stats-api-openapi.yml
- filename: podcastindex-value-api-openapi.yml
  format: yaml
  label: PodcastIndex Value API
  slug: podcastindex-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/openapi/podcastindex-value-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Podcastindex Authentication
name_suffix: Authentication
oauth_flows: []
overview: PodcastIndex secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PodcastIndex
provider_slug: podcastindex
scheme_count: 4
schemes:
- description: 'Please identify the system/product you are using to make this request.



    *Example*: `SuperPodcastPlayer/1.3`'
  in: header
  name: User-Agent
  parameter: User-Agent
  sources:
  - openapi/podcastindex-openapi.yml
  type: apiKey
- description: 'Your API key string



    *Example*: `UXKCGDSYGUUEVQJSYDZH`'
  in: header
  name: API-Key
  parameter: X-Auth-Key
  sources:
  - openapi/podcastindex-openapi.yml
  type: apiKey
- description: 'The current UTC unix epoch time as a string. 3 minute window.



    This value is an integer; round down if needed. The value shall not include a decimal point.



    Value generated should match the value shown on the website https://www.epochconverter.com/.



    *Example*: `1613713388`'
  in: header
  name: Date
  parameter: X-Auth-Date
  sources:
  - openapi/podcastindex-openapi.yml
  type: apiKey
- description: "A SHA-1 hash of the `X-Auth-Key`, the corresponding secret and the `X-Auth-Date` value concatenated as a string.\nThe resulting hash should be encoded as a hexadecimal value, two digits per byte, using lower case letters for\nthe hex digits \"a\" through \"f\".\n\n\nThe Authorization header is computed with something like this (pseudo-code):\n\n    authHeader = sha1(apiKey+apiSecret+unixTime)\n\nExample value,"
  in: header
  name: Authorization
  parameter: Authorization
  sources:
  - openapi/podcastindex-openapi.yml
  type: apiKey
slug: podcastindex-authentication
source_filename: podcastindex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/podcastindex-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: User-Agent\n  type: apiKey\n  in: header\n  parameter: User-Agent\n  description: |-\n    Please identify the system/product you are using to make this request.\n\n\n    *Example*: `SuperPodcastPlayer/1.3`\n  sources:\n  - openapi/podcastindex-openapi.yml\n- name: API-Key\n  type: apiKey\n  in: header\n  parameter: X-Auth-Key\n  description: |-\n    Your API key string\n\n\n    *Example*: `UXKCGDSYGUUEVQJSYDZH`\n  sources:\n  - openapi/podcastindex-openapi.yml\n- name: Date\n  type: apiKey\n  in: header\n  parameter: X-Auth-Date\n  description: |-\n    The current UTC unix epoch time as a string. 3 minute window.\n\n\n    This value is an integer; round down if needed. The value shall not include a decimal point.\n\n\n    Value generated should match the value shown on the website https://www.epochconverter.com/.\n\n\
  \n    *Example*: `1613713388`\n  sources:\n  - openapi/podcastindex-openapi.yml\n- name: Authorization\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    A SHA-1 hash of the `X-Auth-Key`, the corresponding secret and the `X-Auth-Date` value concatenated as a string.\n    The resulting hash should be encoded as a hexadecimal value, two digits per byte, using lower case letters for\n    the hex digits \"a\" through \"f\".\n\n\n    The Authorization header is computed with something like this (pseudo-code):\n\n        authHeader = sha1(apiKey+apiSecret+unixTime)\n\n    Example value,\n  sources:\n  - openapi/podcastindex-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podcastindex/refs/heads/main/authentication/podcastindex-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Podcasting
- Podcast Index
- Discovery
- Open Data
---
