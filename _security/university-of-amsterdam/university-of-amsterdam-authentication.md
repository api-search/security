---
api_key_in: []
api_specs:
- filename: university-of-amsterdam-llm-gateway-openapi.json
  format: json
  label: UvA/HvA AI Gateway
  slug: llm-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/openapi/university-of-amsterdam-llm-gateway-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: University Of Amsterdam Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Amsterdam secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Amsterdam
provider_slug: university-of-amsterdam
scheme_count: 1
schemes:
- description: 'Institution-issued API key. Also accepted as an OpenAI-style `Authorization: Bearer <key>` header, which is how the institution''s own setup guides in github.com/uva/UvA-HvA-Agentic-Tools instruct staff and students to configure clients.'
  evidence:
  - body: '{"error":{"message":"Authentication Error, No api key passed in.","type":"auth_error","code":"401"}}'
    observed: '2026-08-19'
    status: 401
    url: https://llmproxy.uva.nl/v1/models
  in: header
  name: APIKeyHeader
  parameter: x-litellm-api-key
  sources:
  - https://llmproxy.uva.nl/openapi.json
  type: apiKey
slug: university-of-amsterdam-authentication
source_filename: university-of-amsterdam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: derived\nsource: openapi/_original/university-of-amsterdam-llm-gateway-openapi.json\nx-operator: institution\nnote: >-\n  Derived from the OpenAPI document served by the University of Amsterdam /\n  Amsterdam University of Applied Sciences shared AI gateway at\n  https://llmproxy.uva.nl/openapi.json. The gateway runs LiteLLM on the\n  institution's own Azure estate under uva.nl; the authentication model below is\n  what that deployment actually advertises, probed 2026-08-19.\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-litellm-api-key\n  description: >-\n    Institution-issued API key. Also accepted as an OpenAI-style\n    `Authorization: Bearer <key>` header, which is how the institution's own\n    setup guides in github.com/uva/UvA-HvA-Agentic-Tools instruct staff and\n    students to configure clients.\n  sources:\n  - https://llmproxy.uva.nl/openapi.json\n  evidence:\n  - url:\
  \ https://llmproxy.uva.nl/v1/models\n    status: 401\n    body: '{\"error\":{\"message\":\"Authentication Error, No api key passed in.\",\"type\":\"auth_error\",\"code\":\"401\"}}'\n    observed: '2026-08-19'\nkey_issuance:\n  self_serve: false\n  method: request from faculty IT / proxy administrators\n  audience: University of Amsterdam and Amsterdam University of Applied Sciences students, staff and developers\n  source: https://github.com/uva/UvA-HvA-Agentic-Tools\n  x-operator: institution\nother_surfaces:\n- surface: UvA Library Linked Open Data (TriplyDB)\n  x-operator: tenant\n  scheme: HTTP bearer token issued by the TriplyDB platform\n  note: >-\n    Read access to publicly published datasets requires no authentication. The\n    token model belongs to Triply, not to the institution; recorded here as a\n    relationship, not as the institution's own scheme.\n  source: https://docs.triply.cc/triply-api/\n- surface: UvA timetable (MyTimetable / Eveoh)\n  x-operator: tenant\n  scheme:\
  \ session/OAuth behind institutional SSO\n  evidence:\n  - url: https://rooster.uva.nl/api/schedule\n    status: 401\n    observed: '2026-08-19'\n- surface: Institutional identity provider\n  x-operator: institution\n  scheme: SAML 2.0 (AD FS) via SURFconext, federated into eduGAIN\n  entity_id: http://login.uva.nl/adfs/services/trust\n  metadata: https://login.uva.nl/federationmetadata/2007-06/federationmetadata.xml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-amsterdam/refs/heads/main/authentication/university-of-amsterdam-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- University
- Higher Education
- Education
- Public Research University
- Netherlands
- Europe
- LERU
- Open Data
- Linked Data
- Library
- Research Data
- Research Repository
- Course Catalog
- Identity Federation
- OAI-PMH
- Artificial Intelligence
---
