---
api_key_in:
- header
api_specs:
- filename: qomplement-api-keys-api-openapi.yml
  format: yaml
  label: Qomplement API Keys API
  slug: qomplement-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qomplement/refs/heads/main/openapi/qomplement-api-keys-api-openapi.yml
- filename: qomplement-extract-api-openapi.yml
  format: yaml
  label: Qomplement Extract API
  slug: qomplement-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qomplement/refs/heads/main/openapi/qomplement-extract-api-openapi.yml
- filename: qomplement-fill-excel-api-openapi.yml
  format: yaml
  label: Qomplement Fill Excel API
  slug: qomplement-fill-excel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qomplement/refs/heads/main/openapi/qomplement-fill-excel-api-openapi.yml
- filename: qomplement-fill-pdf-api-openapi.yml
  format: yaml
  label: Qomplement Fill PDF API
  slug: qomplement-fill-pdf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qomplement/refs/heads/main/openapi/qomplement-fill-pdf-api-openapi.yml
- filename: qomplement-health-api-openapi.yml
  format: yaml
  label: Qomplement Health API
  slug: qomplement-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qomplement/refs/heads/main/openapi/qomplement-health-api-openapi.yml
- filename: qomplement-jobs-api-openapi.yml
  format: yaml
  label: Qomplement Jobs API
  slug: qomplement-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qomplement/refs/heads/main/openapi/qomplement-jobs-api-openapi.yml
- filename: qomplement-usage-api-openapi.yml
  format: yaml
  label: Qomplement Usage API
  slug: qomplement-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qomplement/refs/heads/main/openapi/qomplement-usage-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Qomplement Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qomplement secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qomplement
provider_slug: qomplement
scheme_count: 1
schemes:
- format: Bearer <api_key>
  in: header
  issued_from: https://developers.qomplement.com
  key_format: sd_ followed by 48 hexadecimal characters
  key_prefix: sd_
  name: bearerApiKey
  parameter: Authorization
  sources:
  - https://docs.qomplement.com/api/authentication
  type: apiKey
slug: qomplement-authentication
source_filename: qomplement-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/qomplement-openapi-original.json\ndocs: https://docs.qomplement.com/api/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  scheme: bearer\n  oauth2_flows: []\n  note: >-\n    The published OpenAPI declares no securitySchemes; authentication is documented\n    only in the developer docs. All API requests require an API key passed as a\n    Bearer token in the Authorization header.\nschemes:\n- name: bearerApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: \"Bearer <api_key>\"\n  key_prefix: sd_\n  key_format: sd_ followed by 48 hexadecimal characters\n  issued_from: https://developers.qomplement.com\n  sources: [https://docs.qomplement.com/api/authentication]\nunauthorized:\n  statuses: [401, 403]\n  message: Could not validate credentials\nnotes:\n  - No sandbox / separate test vs live key prefix is documented.\n  - Keys are shown only once at creation and carry per-minute\
  \ and monthly limits.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qomplement/refs/heads/main/authentication/qomplement-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Document Extraction
- OCR
- Structured Data
- Artificial Intelligence
- Forms Automation
- PDF
- Supply Chain
- Developer API
- Y Combinator
---
