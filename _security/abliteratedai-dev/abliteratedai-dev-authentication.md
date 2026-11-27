---
anonymous_access: false
api_key_in: []
api_specs:
- filename: abliteratedai-dev-openapi-generated.yml
  format: yaml
  label: AbliteratedAI Chat Completions API
  slug: abliteratedai-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abliteratedai-dev/openapi/_ae-authored/abliteratedai-dev-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AbliteratedAI Authentication
name_suffix: Authentication
oauth_flows: []
overview: AbliteratedAI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AbliteratedAI
provider_slug: abliteratedai-dev
scheme_count: 1
schemes:
- header: 'Authorization: Bearer $ABLITERATED_API_KEY'
  key_prefix: abl-sk-
  name: bearer
  notes: Keys start with abl-sk-. The full key is shown once; only a hash and safe prefix are retained. Approval and verified email are required. Revoking or rotating a key invalidates it immediately for new requests.
  scheme: bearer
  scoped_to: project
  type: http
slug: abliteratedai-dev-authentication
source_filename: abliteratedai-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: searched\nsource: https://abliteratedai.dev/docs/authentication\ndocs: https://abliteratedai.dev/docs/authentication\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  header: \"Authorization: Bearer $ABLITERATED_API_KEY\"\n  key_prefix: abl-sk-\n  notes: \"Keys start with abl-sk-. The full key is shown once; only a hash and safe prefix are retained. Approval and verified email are required. Revoking or rotating a key invalidates it immediately for new requests.\"\n  scoped_to: project\n"
source_yaml_url: https://artifacts.apis.io/abliteratedai-dev/authentication/abliteratedai-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- OpenAI-Compatible
- Chat Completions
- Open-Weight
---
