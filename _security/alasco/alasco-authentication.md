---
api_key_in:
- header
api_specs:
- filename: alasco-fincon-openapi.json
  format: json
  label: Alasco FinCon API
  slug: alasco-fincon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/openapi/alasco-fincon-openapi.json
- filename: alasco-capex-openapi.json
  format: json
  label: Alasco CapEx API
  slug: alasco-capex-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/openapi/alasco-capex-openapi.json
- filename: alasco-esg-openapi.json
  format: json
  label: Alasco ESG API
  slug: alasco-esg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/openapi/alasco-esg-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Alasco Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alasco secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Alasco
provider_slug: alasco
scheme_count: 2
schemes:
- description: 'The Alasco API uses a combination of API keys and API tokens to authenticate requests. The API key

    needs to be sent in a header field called `X-API-KEY`.'
  in: header
  name: API Key
  parameter: X-API-KEY
  sources:
  - openapi/alasco-capex-openapi.json
  - openapi/alasco-esg-openapi.json
  - openapi/alasco-fincon-openapi.json
  type: apiKey
- description: 'In addition to an API key, one has to specify an API token. There can be one or more tokens in use

    for the same API key. The token needs to be sent in a header field called `X-API-TOKEN`.

    Right now, it''s not possible to create API keys and API tokens from within Alasco.

    If you are interested in using the Alasco API, please reach out to the

    [support team](mailto:support@alasco.de). They will assist'
  in: header
  name: API Token
  parameter: X-API-TOKEN
  sources:
  - openapi/alasco-capex-openapi.json
  - openapi/alasco-esg-openapi.json
  - openapi/alasco-fincon-openapi.json
  type: apiKey
slug: alasco-authentication
source_filename: alasco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/alasco-capex-openapi.json, openapi/alasco-esg-openapi.json, openapi/alasco-fincon-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: |-\n    The Alasco API uses a combination of API keys and API tokens to authenticate requests. The API key\n    needs to be sent in a header field called `X-API-KEY`.\n  sources:\n  - openapi/alasco-capex-openapi.json\n  - openapi/alasco-esg-openapi.json\n  - openapi/alasco-fincon-openapi.json\n- name: API Token\n  type: apiKey\n  in: header\n  parameter: X-API-TOKEN\n  description: |-\n    In addition to an API key, one has to specify an API token. There can be one or more tokens in use\n    for the same API key. The token needs to be sent in a header field called `X-API-TOKEN`.\n    Right now, it's not possible to create API keys and API tokens from within Alasco.\n  \
  \  If you are interested in using the Alasco API, please reach out to the\n    [support team](mailto:support@alasco.de). They will assist\n  sources:\n  - openapi/alasco-capex-openapi.json\n  - openapi/alasco-esg-openapi.json\n  - openapi/alasco-fincon-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alasco/refs/heads/main/authentication/alasco-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Ai Enterprise Software
- Real Estate
- Construction
- PropTech
- Financial Management
- Cost Management
- Capital Expenditure
- ESG
- Sustainability
---
