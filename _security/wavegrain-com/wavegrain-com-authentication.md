---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wavegrain-com-openapi-generated.yml
  format: yaml
  label: Wavegrain API
  slug: wavegrain-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wavegrain-com/openapi/_ae-authored/wavegrain-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Wavegrain APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Wavegrain Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wavegrain declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Wavegrain
provider_slug: wavegrain-com
scheme_count: 2
schemes:
- evidence: 'Every request to https://wavegrain.com/api/mcp carries a token in the Authorization: Bearer header.'
  header: Authorization
  how_to_obtain: Create in Settings → Connect an AI agent; copy the key that starts with wg_pat_
  location: header
  name: Access key
  type: http-bearer
- authorize_url: https://wavegrain.com/oauth/authorize
  evidence: Hosted apps such as claude.ai cannot store a key, so they sign in with OAuth 2.1 instead.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Register at https://wavegrain.com/oauth/register, then follow the authorization code flow with PKCE to obtain a token that starts with wg_oat_
  location: header
  name: OAuth 2.1
  scopes:
  - read
  - write
  - generate
  - post
  - approve
  type: oauth2
slug: wavegrain-com-authentication
source_filename: wavegrain-com-authentication.yml
source_heading: Authentication Profile
source_url: https://wavegrain.com/developers/api-reference#tag/oauth
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://wavegrain.com/developers/api-reference#tag/oauth\nsources:\n- https://wavegrain.com/developers/api-reference#tag/oauth\n- https://wavegrain.com/developers/api-reference\n- https://wavegrain.com/developers/authentication\n- https://wavegrain.com/developers/authentication.md\ndescription: Authentication methods for Wavegrain APIs\nschemes:\n- type: http-bearer\n  name: Access key\n  evidence: 'Every request to https://wavegrain.com/api/mcp carries a token in the Authorization: Bearer header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create in Settings → Connect an AI agent; copy the key that starts with wg_pat_\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Hosted apps such as claude.ai cannot store a key, so they sign in with OAuth 2.1 instead.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://wavegrain.com/oauth/authorize\n\
  \  scopes:\n  - read\n  - write\n  - generate\n  - post\n  - approve\n  how_to_obtain: Register at https://wavegrain.com/oauth/register, then follow the authorization code flow with PKCE to obtain a token that starts\n    with wg_oat_\ndocs: https://wavegrain.com/developers/api-reference#tag/oauth\n"
source_yaml_url: https://artifacts.apis.io/wavegrain-com/authentication/wavegrain-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Automation
- Social Media
- TikTok
- Instagram
---
