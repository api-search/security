---
anonymous_access: false
api_key_in: []
api_specs:
- filename: avacast-jp-openapi-generated.yml
  format: yaml
  label: avacast-jp API
  slug: avacast-jp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/avacast-jp/openapi/_ae-authored/avacast-jp-openapi-generated.yml
auth_types: []
description: Authentication via API key issued in the Avacast management console.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Avacast Jp Authentication
name_suffix: Authentication
oauth_flows: []
overview: avacast-jp declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: avacast-jp
provider_slug: avacast-jp
scheme_count: 1
schemes:
- evidence: サーバーから avacast の API を呼ぶときに使います。
  how_to_obtain: Issued from the Avacast management console under the API Keys section by the owner.
  name: API key
  type: apiKey
slug: avacast-jp-authentication
source_filename: avacast-jp-authentication.yml
source_heading: Authentication Profile
source_url: https://avacast.jp/docs/guide/api-keys
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://avacast.jp/docs/guide/api-keys\nsources:\n- https://avacast.jp/docs/guide/api-keys\ndescription: Authentication via API key issued in the Avacast management console.\nschemes:\n- type: apiKey\n  name: API key\n  evidence: サーバーから avacast の API を呼ぶときに使います。\n  how_to_obtain: Issued from the Avacast management console under the API Keys section by the owner.\nnote: The page does not specify the exact header name or query parameter used for the API key.\ndocs: https://avacast.jp/docs/guide/api-keys\n"
source_yaml_url: https://artifacts.apis.io/avacast-jp/authentication/avacast-jp-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Avatar
- Real-time
- Japan
---
