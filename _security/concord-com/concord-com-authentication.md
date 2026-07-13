---
api_key_in: []
api_specs:
- filename: concord-com-openapi.yml
  format: yaml
  label: Concord Agreements API
  slug: concord-com-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-openapi.yml
- filename: concord-com-openapi.yml
  format: yaml
  label: Concord Organizations & Users API
  slug: concord-com-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-openapi.yml
- filename: concord-com-openapi.yml
  format: yaml
  label: Concord Documents & Attachments API
  slug: concord-com-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-openapi.yml
- filename: concord-com-openapi.yml
  format: yaml
  label: Concord Templates API
  slug: concord-com-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/openapi/concord-com-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Concord Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Concord secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Concord
provider_slug: concord-com
scheme_count: 1
schemes:
- description: API key generated inside the Concord account (paid plans only) and sent in the `X-API-KEY` request header. Confirmed against the live production host https://api.concordnow.com/api/rest/1, which returns HTTP 401 `{"statusCode":401,"restCode":"unauthorized"}` when called without a valid key.
  in: header
  keyName: X-API-KEY
  name: apiKeyAuth
  sources:
  - openapi/concord-com-openapi.yml
  - https://help.concord.app/concord-api
  type: apiKey
slug: concord-com-authentication
source_filename: concord-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/concord-com-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  keyName: X-API-KEY\n  description: >-\n    API key generated inside the Concord account (paid plans only) and sent in\n    the `X-API-KEY` request header. Confirmed against the live production host\n    https://api.concordnow.com/api/rest/1, which returns HTTP 401\n    `{\"statusCode\":401,\"restCode\":\"unauthorized\"}` when called without a valid\n    key.\n  sources:\n  - openapi/concord-com-openapi.yml\n  - https://help.concord.app/concord-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concord-com/refs/heads/main/authentication/concord-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Contract Management
- Contract Lifecycle Management
- CLM
- Contracts
- Agreements
- E-Signature
- Document Management
- Legal
- Workflow
---
