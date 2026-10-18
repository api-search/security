---
anonymous_access: false
api_key_in: []
api_specs:
- filename: toneperfect-assessment-api-openapi.yml
  format: yaml
  label: TonePerfect (Pronunciation Assessment API) Assessment API
  slug: toneperfect-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toneperfect/refs/heads/main/openapi/toneperfect-assessment-api-openapi.yml
- filename: toneperfect-capabilities-api-openapi.yml
  format: yaml
  label: TonePerfect (Pronunciation Assessment API) Capabilities API
  slug: toneperfect-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toneperfect/refs/heads/main/openapi/toneperfect-capabilities-api-openapi.yml
- filename: toneperfect-utilities-api-openapi.yml
  format: yaml
  label: TonePerfect (Pronunciation Assessment API) Utilities API
  slug: toneperfect-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toneperfect/refs/heads/main/openapi/toneperfect-utilities-api-openapi.yml
auth_types: []
description: Authentication for TonePerfect Pronunciation Assessment API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Toneperfect Authentication
name_suffix: Authentication
oauth_flows: []
overview: TonePerfect (Pronunciation Assessment API) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: TonePerfect (Pronunciation Assessment API)
provider_slug: toneperfect
scheme_count: 1
schemes:
- evidence: Create an account , open API keys in the dashboard and create a key. It starts with tp_live_ and is shown once.
  header: Authorization
  how_to_obtain: Create an account, open API keys in the dashboard and create a key.
  location: header
  name: Bearer
  type: http-bearer
slug: toneperfect-authentication
source_filename: toneperfect-authentication.yml
source_heading: Authentication Profile
source_url: https://api.toneperfect.app/quickstart/
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.toneperfect.app/quickstart/\nsources:\n- https://api.toneperfect.app/quickstart/\ndescription: Authentication for TonePerfect Pronunciation Assessment API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Create an account , open API keys in the dashboard and create a key. It starts with tp_live_ and is shown once.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an account, open API keys in the dashboard and create a key.\ndocs: https://api.toneperfect.app/quickstart/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toneperfect/refs/heads/main/authentication/toneperfect-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Speech
- Language-Learning
- Pronunciation
---
