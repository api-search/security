---
api_key_in:
- query
- header
api_specs:
- filename: misoai-openapi-original.json
  format: json
  label: Miso API
  slug: miso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/openapi/misoai-openapi-original.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Misoai Authentication
name_suffix: Authentication
oauth_flows: []
overview: miso.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: miso.ai
provider_slug: misoai
scheme_count: 1
schemes:
- description: "Your secret API key is used to access every Miso API endpoint. You should secure this key and only use it on a backend \nserver. Never leave this key in your client-side JavaScript code. If the private key is compromised, you can revoke it \nin [Dojo](https://dojo.askmiso.com/docs/api-browser) and get a new one.\n\nSpecify your secret key in the `api_key` query parameter. For example:\n```\nPOST /v1/use"
  in: query
  name: Secret API Key
  parameter: api_key
  sources:
  - openapi/misoai-openapi-original.json
  type: apiKey
slug: misoai-authentication
source_filename: misoai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/misoai-openapi-original.json\ndocs: https://docs.miso.ai/api-reference/authentication\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  - header\n  key_types:\n  - {name: secret, access: full, usage: server-side only}\n  - {name: publishable, access: interaction streaming + read-only search/recs, usage: front-end (user_id must be hashed)}\n  transports:\n  - api_key query parameter (e.g. ?api_key=...)\n  - X-API-KEY request header\n  management: Keys are issued, rotated, and revoked in the Dojo console (https://dojo.miso.ai).\nschemes:\n- name: Secret API Key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: \"Your secret API key is used to access every Miso API endpoint. You should secure\\\n    \\ this key and only use it on a backend \\nserver. Never leave this key in your client-side\\\n    \\ JavaScript code. If the private key is compromised, you can revoke it \\nin [Dojo](https://dojo.askmiso.com/docs/api-browser)\\\
  \n    \\ and get a new one.\\n\\nSpecify your secret key in the `api_key` query parameter. For example:\\n\\\n    ```\\nPOST /v1/use\"\n  sources:\n  - openapi/misoai-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/misoai/refs/heads/main/authentication/misoai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Search
- Recommendations
- Personalization
- Semantic Search
- LLM
- Question Answering
- Publishing
- Media
- Retail
- Ecommerce
- Developers
---
