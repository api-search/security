---
api_key_in: []
api_specs:
- filename: oracle-integration-developer-api.yaml
  format: yaml
  label: Oracle Integration Developer API
  slug: oracle-integration-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/openapi/oracle-integration-developer-api.yaml
- filename: oracle-integration-process-automation-api.yaml
  format: yaml
  label: Oracle Integration Process Automation API
  slug: oracle-integration-process-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/openapi/oracle-integration-process-automation-api.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Integration Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Oracle Integration secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Oracle Integration
provider_slug: oracle-integration
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication via Oracle Identity Cloud Service (IDCS).
  flows:
  - authorizationUrl: https://{idcs-url}/oauth2/v1/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://{idcs-url}/oauth2/v1/token
  name: oauth2
  sources:
  - openapi/oracle-integration-developer-api.yaml
  - openapi/oracle-integration-process-automation-api.yaml
  type: oauth2
- description: Basic authentication with Oracle Integration credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/oracle-integration-developer-api.yaml
  - openapi/oracle-integration-process-automation-api.yaml
  type: http
slug: oracle-integration-authentication
source_filename: oracle-integration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-integration-developer-api.yaml, openapi/oracle-integration-process-automation-api.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{idcs-url}/oauth2/v1/authorize\n    tokenUrl: https://{idcs-url}/oauth2/v1/token\n    scopes: 1\n  description: OAuth 2.0 authentication via Oracle Identity Cloud Service (IDCS).\n  sources:\n  - openapi/oracle-integration-developer-api.yaml\n  - openapi/oracle-integration-process-automation-api.yaml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication with Oracle Integration credentials.\n  sources:\n  - openapi/oracle-integration-developer-api.yaml\n  - openapi/oracle-integration-process-automation-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-integration/refs/heads/main/authentication/oracle-integration-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- API Management
- Automation
- B2B Integration
- Cloud Integration
- Enterprise Integration
- Integration
- iPaaS
- Process Automation
---
