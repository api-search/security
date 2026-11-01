---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Savedthat App Authentication
name_suffix: Authentication
oauth_flows: []
overview: savedthat-app declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: savedthat-app
provider_slug: savedthat-app
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Supabase-issued access token. Discover the authorization server via /.well-known/oauth-protected-resource (issuer: https://igsmkyifxygxogpeagjp.supabase.co/auth/v1).'
  scheme: bearer
  type: http
slug: savedthat-app-authentication
source_filename: savedthat-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: savedthat-app\ngenerated: '2026-10-30'\nmethod: derived\nsource: openapi/savedthat-app-openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: \"Supabase-issued access token. Discover the authorization server via /.well-known/oauth-protected-resource (issuer: https://igsmkyifxygxogpeagjp.supabase.co/auth/v1).\"\n"
source_yaml_url: https://artifacts.apis.io/savedthat-app/authentication/savedthat-app-authentication.yml
summary_line: 1 scheme
tags:
- Video
- AI
- Search
- Transcription
- Productivity
---
