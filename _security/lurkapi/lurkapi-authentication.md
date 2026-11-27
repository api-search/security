---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lurkapi-account-api-openapi.yml
  format: yaml
  label: LurkAPI Account API
  slug: lurkapi-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-account-api-openapi.yml
- filename: lurkapi-bluesky-api-openapi.yml
  format: yaml
  label: LurkAPI Bluesky API
  slug: lurkapi-bluesky-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-bluesky-api-openapi.yml
- filename: lurkapi-ebay-api-openapi.yml
  format: yaml
  label: LurkAPI eBay API
  slug: lurkapi-ebay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-ebay-api-openapi.yml
- filename: lurkapi-facebook-api-openapi.yml
  format: yaml
  label: LurkAPI Facebook API
  slug: lurkapi-facebook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-facebook-api-openapi.yml
- filename: lurkapi-google-api-openapi.yml
  format: yaml
  label: LurkAPI Google API
  slug: lurkapi-google-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-google-api-openapi.yml
- filename: lurkapi-instagram-api-openapi.yml
  format: yaml
  label: LurkAPI Instagram API
  slug: lurkapi-instagram-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-instagram-api-openapi.yml
- filename: lurkapi-link-in-bio-api-openapi.yml
  format: yaml
  label: LurkAPI Link In Bio API
  slug: lurkapi-link-in-bio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-link-in-bio-api-openapi.yml
- filename: lurkapi-reddit-api-openapi.yml
  format: yaml
  label: LurkAPI Reddit API
  slug: lurkapi-reddit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-reddit-api-openapi.yml
- filename: lurkapi-snapchat-api-openapi.yml
  format: yaml
  label: LurkAPI Snapchat API
  slug: lurkapi-snapchat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-snapchat-api-openapi.yml
- filename: lurkapi-telegram-api-openapi.yml
  format: yaml
  label: LurkAPI Telegram API
  slug: lurkapi-telegram-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-telegram-api-openapi.yml
- filename: lurkapi-threads-api-openapi.yml
  format: yaml
  label: LurkAPI Threads API
  slug: lurkapi-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-threads-api-openapi.yml
- filename: lurkapi-tiktok-api-openapi.yml
  format: yaml
  label: LurkAPI Tik Tok API
  slug: lurkapi-tiktok-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-tiktok-api-openapi.yml
- filename: lurkapi-web-api-openapi.yml
  format: yaml
  label: LurkAPI Web API
  slug: lurkapi-web-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-web-api-openapi.yml
- filename: lurkapi-x-twitter-api-openapi.yml
  format: yaml
  label: LurkAPI X (Twitter) API
  slug: lurkapi-x-twitter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-x-twitter-api-openapi.yml
- filename: lurkapi-youtube-api-openapi.yml
  format: yaml
  label: LurkAPI YouTube API
  slug: lurkapi-youtube-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-youtube-api-openapi.yml
- filename: lurkapi-linked-in-api-openapi.yml
  format: yaml
  label: LurkAPI Linked In API
  slug: lurkapi-linked-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-linked-in-api-openapi.yml
- filename: lurkapi-truthsocial-api-openapi.yml
  format: yaml
  label: LurkAPI Truthsocial API
  slug: lurkapi-truthsocial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lurkapi/openapi/lurkapi-truthsocial-api-openapi.yml
auth_types: []
description: Authentication methods for LurkAPI as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LurkAPI Authentication
name_suffix: Authentication
oauth_flows: []
overview: LurkAPI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LurkAPI
provider_slug: lurkapi
scheme_count: 2
schemes:
- evidence: You send it with every request, so we know the call is yours.
  header: x-api-key
  how_to_obtain: Create a key on your dashboard after signing in.
  location: header
  name: x-api-key
  type: apiKey
- evidence: Paste this address, pick OAuth and sign in.
  how_to_obtain: Sign in via the MCP OAuth flow; specific URLs not provided.
  name: OAuth
  type: oauth2
slug: lurkapi-authentication
source_filename: lurkapi-authentication.yml
source_heading: Authentication Profile
source_url: https://lurkapi.com/docs.md
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lurkapi.com/docs.md\nsources:\n- https://lurkapi.com/docs.md\n- https://lurkapi.com/docs\ndescription: Authentication methods for LurkAPI as documented.\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: You send it with every request, so we know the call is yours.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a key on your dashboard after signing in.\n- type: oauth2\n  name: OAuth\n  evidence: Paste this address, pick OAuth and sign in.\n  how_to_obtain: Sign in via the MCP OAuth flow; specific URLs not provided.\ndocs: https://lurkapi.com/docs.md\n"
source_yaml_url: https://artifacts.apis.io/lurkapi/authentication/lurkapi-authentication.yml
summary_line: 2 schemes
tags:
- Social Media
- Data API
- AI Integration
- Advertising
- Analytics
---
