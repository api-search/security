---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Genhealthai Authentication
name_suffix: Authentication
oauth_flows: []
overview: GenHealth.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GenHealth.ai
provider_slug: genhealthai
scheme_count: 1
schemes:
- description: API key passed as a Bearer token in the Authorization request header.
  name: HTTPBearer
  scheme: bearer
  sources:
  - https://docs.genhealth.ai/docs/getting-started-1
  type: http
slug: genhealthai-authentication
source_filename: genhealthai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.genhealth.ai/docs/getting-started-1\ndocs: https://docs.genhealth.ai/docs/getting-started-1\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  oauth2_flows: []\n  api_key_in: []\n  notes: >-\n    GenHealth API requests authenticate with an HTTP Bearer token (an API key issued in the developer\n    hub and sent in the Authorization header). The ReadMe developer hub declares a single security\n    scheme \"HTTPBearer\" (type: http, scheme: bearer) and explicitly no OAuth (oauth type: none).\nschemes:\n  - name: HTTPBearer\n    type: http\n    scheme: bearer\n    description: API key passed as a Bearer token in the Authorization request header.\n    sources:\n      - https://docs.genhealth.ai/docs/getting-started-1\noauth:\n  present: false\n  evidence: developer-hub metadata declares oauth type \"none\"\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genhealthai/refs/heads/main/authentication/genhealthai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Health
- Healthcare
- Artificial Intelligence
- Generative AI
- Prior Authorization
- Revenue Cycle Management
- FHIR
- HL7 Da Vinci
- Medical Coding
- Utilization Management
---
