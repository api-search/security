---
anonymous_access: false
api_key_in: []
api_specs:
- filename: equativ-deals-api-openapi.yml
  format: yaml
  label: Equativ Deals API
  slug: equativ-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equativ/refs/heads/main/openapi/equativ-deals-api-openapi.yml
- filename: equativ-regions-api-openapi.yml
  format: yaml
  label: Equativ Regions API
  slug: equativ-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equativ/refs/heads/main/openapi/equativ-regions-api-openapi.yml
- filename: equativ-semanticsegmentproviders-api-openapi.yml
  format: yaml
  label: Equativ Semanticsegmentproviders API
  slug: equativ-semanticsegmentproviders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equativ/refs/heads/main/openapi/equativ-semanticsegmentproviders-api-openapi.yml
- filename: equativ-semanticsegments-api-openapi.yml
  format: yaml
  label: Equativ Semanticsegments API
  slug: equativ-semanticsegments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equativ/refs/heads/main/openapi/equativ-semanticsegments-api-openapi.yml
- filename: equativ-states-api-openapi.yml
  format: yaml
  label: Equativ States API
  slug: equativ-states-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equativ/refs/heads/main/openapi/equativ-states-api-openapi.yml
- filename: equativ-videoadbreaktypes-api-openapi.yml
  format: yaml
  label: Equativ Videoadbreaktypes API
  slug: equativ-videoadbreaktypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equativ/refs/heads/main/openapi/equativ-videoadbreaktypes-api-openapi.yml
- filename: equativ-videoplacementtypes-api-openapi.yml
  format: yaml
  label: Equativ Videoplacementtypes API
  slug: equativ-videoplacementtypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/equativ/refs/heads/main/openapi/equativ-videoplacementtypes-api-openapi.yml
auth_types: []
description: Authentication for Equativ SSAI endpoints uses a dedicated API key generated per stream, which must be included as the `api-key` query parameter in each request.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Equativ Authentication
name_suffix: Authentication
oauth_flows: []
overview: Equativ declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Equativ
provider_slug: equativ
scheme_count: 1
schemes:
- evidence: For each SSAI-enabled stream (VoD endpoint or live channel), a dedicated API key is generated. This key is required for every playback request and must be included in the URL as the api-key parameter.
  how_to_obtain: The API key is obtained from the channel configuration in Serverside.ai.
  location: query
  name: api-key
  type: apiKey
slug: equativ-authentication
source_filename: equativ-authentication.yml
source_heading: Authentication Profile
source_url: https://help.equativ.com/en_US/ssai-authentication/ssai-authentication
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.equativ.com/en_US/ssai-authentication/ssai-authentication\nsources:\n- https://help.equativ.com/en_US/ssai-authentication/ssai-authentication\n- https://help.equativ.com/en_US/ssai-authentication/live-dash-and-hls\n- https://help.equativ.com/en_US/ssai-authentication/vod-dash-hls\n- https://help.equativ.com/en_US/ssai-authentication/vast-tracking\ndescription: Authentication for Equativ SSAI endpoints uses a dedicated API key generated per stream, which must be included as the `api-key`\n  query parameter in each request.\nschemes:\n- type: apiKey\n  name: api-key\n  evidence: For each SSAI-enabled stream (VoD endpoint or live channel), a dedicated API key is generated. This key is required for every playback\n    request and must be included in the URL as the api-key parameter.\n  location: query\n  how_to_obtain: The API key is obtained from the channel configuration\
  \ in Serverside.ai.\ndocs: https://help.equativ.com/en_US/ssai-authentication/ssai-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/equativ/refs/heads/main/authentication/equativ-authentication.yml
summary_line: 1 scheme
tags:
- Advertising
- Media
- Technology
- Retail
- Platform
---
