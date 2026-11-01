---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datalikers-com-comment-api-openapi.yml
  format: yaml
  label: datalikers-com Comment API
  slug: datalikers-com-comment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-comment-api-openapi.yml
- filename: datalikers-com-hashtag-api-openapi.yml
  format: yaml
  label: datalikers-com Hashtag API
  slug: datalikers-com-hashtag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-hashtag-api-openapi.yml
- filename: datalikers-com-highlight-api-openapi.yml
  format: yaml
  label: datalikers-com Highlight API
  slug: datalikers-com-highlight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-highlight-api-openapi.yml
- filename: datalikers-com-location-api-openapi.yml
  format: yaml
  label: datalikers-com Location API
  slug: datalikers-com-location-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-location-api-openapi.yml
- filename: datalikers-com-media-api-openapi.yml
  format: yaml
  label: datalikers-com Media API
  slug: datalikers-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-media-api-openapi.yml
- filename: datalikers-com-story-api-openapi.yml
  format: yaml
  label: datalikers-com Story API
  slug: datalikers-com-story-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-story-api-openapi.yml
- filename: datalikers-com-system-api-openapi.yml
  format: yaml
  label: datalikers-com System API
  slug: datalikers-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-system-api-openapi.yml
- filename: datalikers-com-tiktok-comment-api-openapi.yml
  format: yaml
  label: datalikers-com TikTok Comment API
  slug: datalikers-com-tiktok-comment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-tiktok-comment-api-openapi.yml
- filename: datalikers-com-tiktok-hashtag-api-openapi.yml
  format: yaml
  label: datalikers-com TikTok Hashtag API
  slug: datalikers-com-tiktok-hashtag-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-tiktok-hashtag-api-openapi.yml
- filename: datalikers-com-tiktok-media-api-openapi.yml
  format: yaml
  label: datalikers-com TikTok Media API
  slug: datalikers-com-tiktok-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-tiktok-media-api-openapi.yml
- filename: datalikers-com-tiktok-playlist-api-openapi.yml
  format: yaml
  label: datalikers-com TikTok Playlist API
  slug: datalikers-com-tiktok-playlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-tiktok-playlist-api-openapi.yml
- filename: datalikers-com-tiktok-user-api-openapi.yml
  format: yaml
  label: datalikers-com TikTok User API
  slug: datalikers-com-tiktok-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-tiktok-user-api-openapi.yml
- filename: datalikers-com-track-api-openapi.yml
  format: yaml
  label: datalikers-com Track API
  slug: datalikers-com-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-track-api-openapi.yml
- filename: datalikers-com-user-api-openapi.yml
  format: yaml
  label: datalikers-com User API
  slug: datalikers-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-user-api-openapi.yml
- filename: datalikers-com-user-v2-api-openapi.yml
  format: yaml
  label: datalikers-com User v2 API
  slug: datalikers-com-user-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datalikers-com/openapi/datalikers-com-user-v2-api-openapi.yml
auth_types: []
description: DataLikers uses OAuth 2.0 for client authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Datalikers Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: datalikers-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: datalikers-com
provider_slug: datalikers-com
scheme_count: 1
schemes:
- authorize_url: https://datalikers.com/oauth/authorize
  evidence: DataLikers requires PKCE with S256 (RFC 7636); the request must include code_challenge and code_challenge_method=S256.
  flows:
  - authorization_code
  how_to_obtain: Register a client at https://datalikers.com/oauth/register to receive a client_id and client_secret.
  name: OAuth 2.0
  type: oauth2
slug: datalikers-com-authentication
source_filename: datalikers-com-authentication.yml
source_heading: Authentication Profile
source_url: https://datalikers.com/help/oauth-troubleshooting
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://datalikers.com/help/oauth-troubleshooting\nsources:\n- https://datalikers.com/help/oauth-troubleshooting\n- https://datalikers.com/help/oauth-troubleshooting.md\ndescription: DataLikers uses OAuth 2.0 for client authentication.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: DataLikers requires PKCE with S256 (RFC 7636); the request must include code_challenge and code_challenge_method=S256.\n  flows:\n  - authorization_code\n  authorize_url: https://datalikers.com/oauth/authorize\n  how_to_obtain: Register a client at https://datalikers.com/oauth/register to receive a client_id and client_secret.\nnote: Token endpoint is https://datalikers.com/oauth/token (used for token exchange).\ndocs: https://datalikers.com/help/oauth-troubleshooting\n"
source_yaml_url: https://artifacts.apis.io/datalikers-com/authentication/datalikers-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data
- Social Media
- API
- Developer Platform
---
