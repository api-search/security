---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Causaly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Causaly secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Causaly
provider_slug: causaly
scheme_count: 1
schemes:
- applies_to: Bio Graph API
  description: Enterprise-issued API token used to authenticate Bio Graph API requests and the R/Python client libraries.
  in: header
  name: apiToken
  source: https://www.causaly.com/products/bio-graph-api
  type: apiKey
slug: causaly-authentication
source_filename: causaly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://www.causaly.com/products/bio-graph-api\ndocs: https://www.causaly.com/products/bio-graph-api\n# No public OpenAPI is published, so this profile is captured from the Bio Graph\n# API product page, which documents access via \"Simple API token, pre-made\n# templates, and R/Python libraries.\" The token is issued to enterprise\n# customers; there is no public self-serve auth flow or documented OAuth surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  applies_to: Bio Graph API\n  description: Enterprise-issued API token used to authenticate Bio Graph API requests and the R/Python client libraries.\n  source: https://www.causaly.com/products/bio-graph-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/causaly/refs/heads/main/authentication/causaly-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- Life Sciences
- Biomedical
- Drug Discovery
- Knowledge Graph
- Pharmaceutical
- Research
- Agentic AI
---
