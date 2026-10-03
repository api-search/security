---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arcmira-v1-openapi.json
  format: json
  label: Arcmira API V1 API
  slug: arcmira-api-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/_original/arcmira-v1-openapi.json
auth_types: []
description: Authentication schemes for Arcmira API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Arcmira Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arcmira declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Arcmira
provider_slug: arcmira
scheme_count: 1
schemes:
- evidence: 'Pass your key as a bearer token:'
  header: Authorization
  how_to_obtain: Create a key in the Dashboard → API Keys page; the key has the prefix arc_sk_ and is used as the bearer token.
  location: header
  name: API Key
  type: http-bearer
slug: arcmira-authentication
source_filename: arcmira-authentication.yml
source_heading: Authentication Profile
source_url: https://arcmira.com/docs/authentication.md#sign-up-from-the-api
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://arcmira.com/docs/authentication.md#sign-up-from-the-api\nsources:\n- https://arcmira.com/docs/authentication.md#sign-up-from-the-api\n- https://arcmira.com/docs/authentication.md\n- https://arcmira.com/docs/authentication\ndescription: Authentication schemes for Arcmira API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Pass your key as a bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the Dashboard → API Keys page; the key has the prefix arc_sk_ and is used as the bearer token.\ndocs: https://arcmira.com/docs/authentication.md#sign-up-from-the-api\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/authentication/arcmira-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Search
- YouTube
- Transcripts
- SDK
---
