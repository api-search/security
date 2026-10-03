---
anonymous_access: false
api_key_in: []
api_specs:
- filename: posteahora-accounts-api-openapi.yml
  format: yaml
  label: PosteAhora Accounts API
  slug: posteahora-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posteahora/refs/heads/main/openapi/posteahora-accounts-api-openapi.yml
- filename: posteahora-analytics-api-openapi.yml
  format: yaml
  label: PosteAhora Analytics API
  slug: posteahora-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posteahora/refs/heads/main/openapi/posteahora-analytics-api-openapi.yml
- filename: posteahora-ideas-api-openapi.yml
  format: yaml
  label: PosteAhora Ideas API
  slug: posteahora-ideas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posteahora/refs/heads/main/openapi/posteahora-ideas-api-openapi.yml
- filename: posteahora-media-api-openapi.yml
  format: yaml
  label: PosteAhora Media API
  slug: posteahora-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posteahora/refs/heads/main/openapi/posteahora-media-api-openapi.yml
- filename: posteahora-posts-api-openapi.yml
  format: yaml
  label: PosteAhora Posts API
  slug: posteahora-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/posteahora/refs/heads/main/openapi/posteahora-posts-api-openapi.yml
auth_types: []
description: Every request is authenticated with a PosteAhora API key, scoped to exactly what the integration needs.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Posteahora Authentication
name_suffix: Authentication
oauth_flows: []
overview: PosteAhora declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PosteAhora
provider_slug: posteahora
scheme_count: 1
schemes:
- evidence: Every request is authenticated with a PosteAhora API key, scoped to exactly what the integration needs.
  header: Authorization
  how_to_obtain: Create keys in the app under API; a key is shown once — store it like a password.
  location: header
  name: API Key
  scopes:
  - ideas:read
  - ideas:write
  - posts:read
  - posts:write
  - analytics:read
  - accounts:read
  - media:write
  type: apiKey
slug: posteahora-authentication
source_filename: posteahora-authentication.yml
source_heading: Authentication Profile
source_url: https://posteahora.com/docs/authentication
source_yaml: "generated: '2026-09-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://posteahora.com/docs/authentication\nsources:\n- https://posteahora.com/docs/authentication\n- https://posteahora.com/docs/quickstart\ndescription: Every request is authenticated with a PosteAhora API key, scoped to exactly what the integration needs.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Every request is authenticated with a PosteAhora API key, scoped to exactly what the integration needs.\n  location: header\n  header: Authorization\n  scopes:\n  - ideas:read\n  - ideas:write\n  - posts:read\n  - posts:write\n  - analytics:read\n  - accounts:read\n  - media:write\n  how_to_obtain: Create keys in the app under API; a key is shown once — store it like a password.\ndocs: https://posteahora.com/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/posteahora/refs/heads/main/authentication/posteahora-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Social Media
- AI Automation
- Marketing
- Software-as-a-Service
---
