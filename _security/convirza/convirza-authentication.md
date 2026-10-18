---
anonymous_access: false
api_key_in: []
api_specs:
- filename: convirza-ad-source-api-openapi.yml
  format: yaml
  label: Convirza Ad Source API
  slug: convirza-ad-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-ad-source-api-openapi.yml
- filename: convirza-ai-voice-agents-api-openapi.yml
  format: yaml
  label: Convirza Ai Voice Agents API
  slug: convirza-ai-voice-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-ai-voice-agents-api-openapi.yml
- filename: convirza-broadcast-api-openapi.yml
  format: yaml
  label: Convirza Broadcast API
  slug: convirza-broadcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-broadcast-api-openapi.yml
- filename: convirza-conversations-api-openapi.yml
  format: yaml
  label: Convirza Conversations API
  slug: convirza-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-conversations-api-openapi.yml
- filename: convirza-convirza-api-api-openapi.yml
  format: yaml
  label: Convirza Convirza API
  slug: convirza-convirza-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-convirza-api-api-openapi.yml
- filename: convirza-groups-api-openapi.yml
  format: yaml
  label: Convirza Groups API
  slug: convirza-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-groups-api-openapi.yml
- filename: convirza-industry-api-openapi.yml
  format: yaml
  label: Convirza Industry API
  slug: convirza-industry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-industry-api-openapi.yml
- filename: convirza-media-prompts-api-openapi.yml
  format: yaml
  label: Convirza Media Prompts API
  slug: convirza-media-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-media-prompts-api-openapi.yml
- filename: convirza-oauth-api-openapi.yml
  format: yaml
  label: Convirza OAuth API
  slug: convirza-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-oauth-api-openapi.yml
- filename: convirza-phone-numbers-api-openapi.yml
  format: yaml
  label: Convirza Phone Numbers API
  slug: convirza-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-phone-numbers-api-openapi.yml
- filename: convirza-provisioned-routes-api-openapi.yml
  format: yaml
  label: Convirza Provisioned Routes API
  slug: convirza-provisioned-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-provisioned-routes-api-openapi.yml
- filename: convirza-tag-api-openapi.yml
  format: yaml
  label: Convirza Tag API
  slug: convirza-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-tag-api-openapi.yml
- filename: convirza-user-api-openapi.yml
  format: yaml
  label: Convirza User API
  slug: convirza-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-user-api-openapi.yml
- filename: convirza-users-api-openapi.yml
  format: yaml
  label: Convirza Users API
  slug: convirza-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-users-api-openapi.yml
- filename: convirza-webhooks-api-openapi.yml
  format: yaml
  label: Convirza Webhooks API
  slug: convirza-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/openapi/convirza-webhooks-api-openapi.yml
auth_types: []
description: Convirza uses encrypted Bearer token authentication and OAuth 2.0 flows.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Convirza Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convirza declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Convirza
provider_slug: convirza
scheme_count: 1
schemes:
- evidence: Convirza uses **encrypted Bearer token authentication** with server-side session storage.
  header: Authorization
  how_to_obtain: Send your credentials to POST /oauth/token and receive an encrypted access_token and refresh_token.
  location: header
  name: Bearer Token
  token_url: /oauth/token
  type: http-bearer
slug: convirza-authentication
source_filename: convirza-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.convirza.com/authentication-2043390m0.md
source_yaml: "generated: '2026-10-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.convirza.com/authentication-2043390m0.md\nsources:\n- https://docs.convirza.com/authentication-2043390m0.md\n- https://docs.convirza.com/authentication-access-2395719m0.md\n- https://docs.convirza.com/working-with-encrypted-tokens-2043382m0.md\n- https://docs.convirza.com/get-access-token-32391152e0.md\ndescription: Convirza uses encrypted Bearer token authentication and OAuth 2.0 flows.\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: Convirza uses **encrypted Bearer token authentication** with server-side session storage.\n  location: header\n  header: Authorization\n  token_url: /oauth/token\n  how_to_obtain: Send your credentials to POST /oauth/token and receive an encrypted access_token and refresh_token.\ndocs: https://docs.convirza.com/authentication-2043390m0.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convirza/refs/heads/main/authentication/convirza-authentication.yml
summary_line: 1 scheme
tags:
- Conversation Analytics
- Call Tracking
- Artificial Intelligence
- Marketing
- Sales Enablement
---
