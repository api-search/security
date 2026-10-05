---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arcmira-channels-api-openapi.yml
  format: yaml
  label: Arcmira Channels API
  slug: arcmira-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/arcmira-channels-api-openapi.yml
- filename: arcmira-entities-api-openapi.yml
  format: yaml
  label: Arcmira Entities API
  slug: arcmira-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/arcmira-entities-api-openapi.yml
- filename: arcmira-feedback-api-openapi.yml
  format: yaml
  label: Arcmira Feedback API
  slug: arcmira-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/arcmira-feedback-api-openapi.yml
- filename: arcmira-mentions-api-openapi.yml
  format: yaml
  label: Arcmira Mentions API
  slug: arcmira-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/arcmira-mentions-api-openapi.yml
- filename: arcmira-meta-api-openapi.yml
  format: yaml
  label: Arcmira Meta API
  slug: arcmira-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/arcmira-meta-api-openapi.yml
- filename: arcmira-monitors-api-openapi.yml
  format: yaml
  label: Arcmira Monitors API
  slug: arcmira-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/arcmira-monitors-api-openapi.yml
- filename: arcmira-recommendations-api-openapi.yml
  format: yaml
  label: Arcmira Recommendations API
  slug: arcmira-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/arcmira-recommendations-api-openapi.yml
- filename: arcmira-search-api-openapi.yml
  format: yaml
  label: Arcmira Search API
  slug: arcmira-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/arcmira-search-api-openapi.yml
- filename: arcmira-trackers-api-openapi.yml
  format: yaml
  label: Arcmira Trackers API
  slug: arcmira-trackers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/arcmira-trackers-api-openapi.yml
- filename: arcmira-transcriptions-api-openapi.yml
  format: yaml
  label: Arcmira Transcriptions API
  slug: arcmira-transcriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/arcmira-transcriptions-api-openapi.yml
- filename: arcmira-transcripts-api-openapi.yml
  format: yaml
  label: Arcmira Transcripts API
  slug: arcmira-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcmira/refs/heads/main/openapi/arcmira-transcripts-api-openapi.yml
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
- Artificial Intelligence
- Search
- YouTube
- Transcripts
- SDK
---
