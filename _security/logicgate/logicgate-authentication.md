---
api_key_in: []
api_specs:
- filename: logicgate-access-audit-api-openapi.yml
  format: yaml
  label: LogicGate Access Audit API
  slug: logicgate-access-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-access-audit-api-openapi.yml
- filename: logicgate-application-api-openapi.yml
  format: yaml
  label: LogicGate Application API
  slug: logicgate-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-application-api-openapi.yml
- filename: logicgate-authentication-api-openapi.yml
  format: yaml
  label: LogicGate Authentication API
  slug: logicgate-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-authentication-api-openapi.yml
- filename: logicgate-edge-path-api-openapi.yml
  format: yaml
  label: LogicGate Edge Path API
  slug: logicgate-edge-path-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-edge-path-api-openapi.yml
- filename: logicgate-field-api-openapi.yml
  format: yaml
  label: LogicGate Field API
  slug: logicgate-field-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-field-api-openapi.yml
- filename: logicgate-next-path-api-openapi.yml
  format: yaml
  label: LogicGate Next Path API
  slug: logicgate-next-path-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-next-path-api-openapi.yml
- filename: logicgate-record-api-openapi.yml
  format: yaml
  label: LogicGate Record API
  slug: logicgate-record-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-record-api-openapi.yml
- filename: logicgate-redirect-path-api-openapi.yml
  format: yaml
  label: LogicGate Redirect Path API
  slug: logicgate-redirect-path-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-redirect-path-api-openapi.yml
- filename: logicgate-step-api-openapi.yml
  format: yaml
  label: LogicGate Step API
  slug: logicgate-step-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-step-api-openapi.yml
- filename: logicgate-workflow-api-openapi.yml
  format: yaml
  label: LogicGate Workflow API
  slug: logicgate-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-workflow-api-openapi.yml
- filename: logicgate-workflow-map-api-openapi.yml
  format: yaml
  label: LogicGate Workflow Map API
  slug: logicgate-workflow-map-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/openapi/logicgate-workflow-map-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Logicgate Authentication
name_suffix: Authentication
oauth_flows: []
overview: LogicGate secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LogicGate
provider_slug: logicgate
scheme_count: 2
schemes:
- bearerFormat: API Token
  name: API Token
  scheme: bearer
  sources:
  - openapi/logicgate-risk-cloud-openapi-original.json
  type: http
- bearerFormat: basic
  name: basic
  scheme: basic
  sources:
  - openapi/logicgate-risk-cloud-openapi-original.json
  type: http
slug: logicgate-authentication
source_filename: logicgate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/logicgate-risk-cloud-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: API Token\n  type: http\n  scheme: bearer\n  bearerFormat: API Token\n  sources:\n  - openapi/logicgate-risk-cloud-openapi-original.json\n- name: basic\n  type: http\n  scheme: basic\n  bearerFormat: basic\n  sources:\n  - openapi/logicgate-risk-cloud-openapi-original.json\ndocs: https://www.logicgate.com/developer/risk-cloud-api-authentication/\ntoken_endpoint: POST /api/v1/account/token (Basic base64(client:secret) -> access_token)\nrefresh_endpoint: POST /api/v2/account/token\ntoken_ttl: ~1 year (expires_in ~31,536,000s)\nscope: read write\nnote: API access requires the paid API Access add-on. Bearer \"API Token\" is the primary\n  scheme; HTTP basic is used only to mint the token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logicgate/refs/heads/main/authentication/logicgate-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- GRC
- Governance Risk and Compliance
- Risk Management
- Compliance
- Workflow Automation
- Audit
- No-Code
---
