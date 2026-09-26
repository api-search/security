---
anonymous_access: false
api_key_in: []
api_specs:
- filename: findlocal-bluesky-api-openapi.yml
  format: yaml
  label: FindLocal Bluesky API
  slug: findlocal-bluesky-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-bluesky-api-openapi.yml
- filename: findlocal-github-api-openapi.yml
  format: yaml
  label: FindLocal GitHub API
  slug: findlocal-github-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-github-api-openapi.yml
- filename: findlocal-history-api-openapi.yml
  format: yaml
  label: FindLocal History API
  slug: findlocal-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-history-api-openapi.yml
- filename: findlocal-instagram-api-openapi.yml
  format: yaml
  label: FindLocal Instagram API
  slug: findlocal-instagram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-instagram-api-openapi.yml
- filename: findlocal-linktree-api-openapi.yml
  format: yaml
  label: FindLocal Linktree API
  slug: findlocal-linktree-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-linktree-api-openapi.yml
- filename: findlocal-mastodon-api-openapi.yml
  format: yaml
  label: FindLocal Mastodon API
  slug: findlocal-mastodon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-mastodon-api-openapi.yml
- filename: findlocal-medium-api-openapi.yml
  format: yaml
  label: FindLocal Medium API
  slug: findlocal-medium-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-medium-api-openapi.yml
- filename: findlocal-movers-api-openapi.yml
  format: yaml
  label: FindLocal Movers API
  slug: findlocal-movers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-movers-api-openapi.yml
- filename: findlocal-events-api-openapi.yml
  format: yaml
  label: FindLocal Events API
  slug: findlocal-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-events-api-openapi.yml
- filename: findlocal-nichos-api-openapi.yml
  format: yaml
  label: FindLocal Nichos API
  slug: findlocal-nichos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-nichos-api-openapi.yml
- filename: findlocal-pinterest-api-openapi.yml
  format: yaml
  label: FindLocal Pinterest API
  slug: findlocal-pinterest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-pinterest-api-openapi.yml
- filename: findlocal-soundcloud-api-openapi.yml
  format: yaml
  label: FindLocal Soundcloud API
  slug: findlocal-soundcloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-soundcloud-api-openapi.yml
- filename: findlocal-threads-api-openapi.yml
  format: yaml
  label: FindLocal Threads API
  slug: findlocal-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-threads-api-openapi.yml
- filename: findlocal-tiktok-api-openapi.yml
  format: yaml
  label: FindLocal Tiktok API
  slug: findlocal-tiktok-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-tiktok-api-openapi.yml
- filename: findlocal-trends-api-openapi.yml
  format: yaml
  label: FindLocal Trends API
  slug: findlocal-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-trends-api-openapi.yml
- filename: findlocal-events-api-openapi.yml
  format: yaml
  label: FindLocal Events API
  slug: findlocal-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-events-api-openapi.yml
- filename: findlocal-venues-api-openapi.yml
  format: yaml
  label: FindLocal Venues API
  slug: findlocal-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/openapi/findlocal-venues-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Findlocal Authentication
name_suffix: Authentication
oauth_flows: []
overview: FindLocal declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FindLocal
provider_slug: findlocal
scheme_count: 1
schemes:
- authorize_url: /authorize
  evidence: 'Auth: OAuth 2.1 with PKCE and dynamic client registration ( /authorize , /token , /register ), then a one-field consent page asking for your API key .'
  flows:
  - authorization_code
  how_to_obtain: Create a free account and make a key in the dashboard.
  name: OAuth 2.1 PKCE
  scopes:
  - mcp:read
  type: oauth2
slug: findlocal-authentication
source_filename: findlocal-authentication.yml
source_heading: Authentication Profile
source_url: https://findlocal.community/login
source_yaml: "generated: '2026-09-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://findlocal.community/login\nsources:\n- https://findlocal.community/login\n- https://findlocal.community/login\n- https://findlocal.community/mcp\nschemes:\n- type: oauth2\n  name: OAuth 2.1 PKCE\n  evidence: 'Auth: OAuth 2.1 with PKCE and dynamic client registration ( /authorize , /token , /register ), then a one-field consent page asking\n    for your API key .'\n  flows:\n  - authorization_code\n  authorize_url: /authorize\n  scopes:\n  - mcp:read\n  how_to_obtain: Create a free account and make a key in the dashboard.\ndocs: https://findlocal.community/login\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/findlocal/refs/heads/main/authentication/findlocal-authentication.yml
summary_line: 1 scheme
tags:
- Events
- API
- Hyperlocal
- Community
- Data
- OpenData
---
