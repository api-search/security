---
anonymous_access: false
api_key_in: []
api_specs:
- filename: audiostack-content-api-openapi.yml
  format: yaml
  label: AudioStack Content API
  slug: audiostack-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiostack/refs/heads/main/openapi/audiostack-content-api-openapi.yml
- filename: audiostack-creator-api-openapi.yml
  format: yaml
  label: AudioStack Creator API
  slug: audiostack-creator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/audiostack/refs/heads/main/openapi/audiostack-creator-api-openapi.yml
auth_types: []
description: AudioStack uses API keys and optionally JWT bearer tokens for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Audiostack Authentication
name_suffix: Authentication
oauth_flows: []
overview: AudioStack declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AudioStack
provider_slug: audiostack
scheme_count: 1
schemes:
- evidence: All requests must be made over HTTPS and will be authenticated using an API key.
  header: x-api-key
  how_to_obtain: Create your API key in the AudioStack Platform.
  location: header
  name: x-api-key
  type: apiKey
slug: audiostack-authentication
source_filename: audiostack-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.audiostack.ai/reference/authentication.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.audiostack.ai/reference/authentication.md\nsources:\n- https://docs.audiostack.ai/reference/authentication.md\n- https://docs.audiostack.ai/reference/gethealth.md\n- https://docs.audiostack.ai/reference/authentication\n- https://docs.audiostack.ai/reference/gethealth\ndescription: AudioStack uses API keys and optionally JWT bearer tokens for authentication.\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: All requests must be made over HTTPS and will be authenticated using an API key.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create your API key in the AudioStack Platform.\nnote: No OAuth2 flows are described on the provided pages. 1 extracted row(s) were dropped because their quote was not on the page.\ndocs: https://docs.audiostack.ai/reference/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audiostack/refs/heads/main/authentication/audiostack-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Audio
- Advertising
- Platform
---
