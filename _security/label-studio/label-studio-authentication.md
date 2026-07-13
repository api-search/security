---
api_key_in:
- header
api_specs:
- filename: label-studio-openapi.yml
  format: yaml
  label: Label Studio
  slug: label-studio
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/label-studio/refs/heads/main/openapi/label-studio-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Label Studio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Label Studio secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Label Studio
provider_slug: label-studio
scheme_count: 1
schemes:
- description: 'The token (or API key) must be passed as a request header. You can find your user token on the User Account page in Label Studio. Example: <br><pre><code class="language-bash">curl https://label-studio-host/api/projects -H "Authorization: Token [your-token]"</code></pre>'
  in: header
  name: Token
  parameter: Authorization
  sources:
  - openapi/label-studio-openapi.yml
  type: apiKey
slug: label-studio-authentication
source_filename: label-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/label-studio-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'The token (or API key) must be passed as a request header. You can find your\n    user token on the User Account page in Label Studio. Example: <br><pre><code class=\"language-bash\">curl\n    https://label-studio-host/api/projects -H \"Authorization: Token [your-token]\"</code></pre>'\n  sources:\n  - openapi/label-studio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/label-studio/refs/heads/main/authentication/label-studio-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI
- Annotation
- Artificial Intelligence
- Data Labeling
- LLM
- Machine Learning
- Open Source
---
