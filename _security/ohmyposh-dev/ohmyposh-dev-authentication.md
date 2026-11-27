---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Oh My Posh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oh My Posh declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Oh My Posh
provider_slug: ohmyposh-dev
scheme_count: 1
schemes:
- evidence: You must request an API key at the wakatime website.
  how_to_obtain: Request an API key from the Wakatime website and include it in the URL query parameter "api_key".
  location: query
  name: Wakatime API Key
  type: apiKey
slug: ohmyposh-dev-authentication
source_filename: ohmyposh-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://ohmyposh.dev/docs/segments/music/lastfm
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ohmyposh.dev/docs/segments/music/lastfm\nsources:\n- https://ohmyposh.dev/docs/segments/music/lastfm\n- https://ohmyposh.dev/docs/segments/web/brewfather\n- https://ohmyposh.dev/docs/segments/web/todoist\n- https://ohmyposh.dev/docs/segments/web/wakatime\nschemes:\n- type: apiKey\n  name: Wakatime API Key\n  evidence: You must request an API key at the wakatime website.\n  location: query\n  how_to_obtain: Request an API key from the Wakatime website and include it in the URL query parameter \"api_key\".\nnote: Other segments (LastFM, Brewfather, Todoist) require API keys but the documentation does not specify where the credentials are sent, so\n  no authentication scheme could be captured.\ndocs: https://ohmyposh.dev/docs/segments/music/lastfm\n"
source_yaml_url: https://artifacts.apis.io/ohmyposh-dev/authentication/ohmyposh-dev-authentication.yml
summary_line: 1 scheme
tags:
- Prompt Engine
- Open Source
- Go
- Cross-Platform
- Shell
---
