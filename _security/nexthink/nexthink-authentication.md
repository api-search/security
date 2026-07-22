---
api_key_in: []
api_specs:
- filename: nexthink-nql-api-openapi.json
  format: json
  label: Nexthink NQL API
  slug: nexthink-nql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-nql-api-openapi.json
- filename: nexthink-remote-actions-api-openapi.json
  format: json
  label: Nexthink Remote Actions API
  slug: nexthink-remote-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-remote-actions-api-openapi.json
- filename: nexthink-workflows-openapi.json
  format: json
  label: Nexthink Workflows API
  slug: nexthink-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-workflows-openapi.json
- filename: nexthink-enrichment-api-openapi.json
  format: json
  label: Nexthink Enrichment API
  slug: nexthink-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-enrichment-api-openapi.json
- filename: nexthink-campaigns-api-openapi.json
  format: json
  label: Nexthink Campaigns API
  slug: nexthink-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-campaigns-api-openapi.json
- filename: nexthink-data-management-api-openapi.json
  format: json
  label: Nexthink Data Management API
  slug: nexthink-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-data-management-api-openapi.json
- filename: nexthink-spark-api-openapi.json
  format: json
  label: Nexthink Spark API
  slug: nexthink-spark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/openapi/nexthink-spark-api-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Nexthink Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Nexthink secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Nexthink
provider_slug: nexthink
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nexthink-campaigns-api-openapi.json
  - openapi/nexthink-data-management-api-openapi.json
  - openapi/nexthink-enrichment-api-openapi.json
  - openapi/nexthink-nql-api-openapi.json
  - openapi/nexthink-remote-actions-api-openapi.json
  - openapi/nexthink-spark-api-openapi.json
  - openapi/nexthink-workflows-openapi.json
  type: http
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://instance-login.region.nexthink.cloud/oauth2/default/v1/token
  name: publicApiAuth
  sources:
  - openapi/nexthink-workflows-openapi.json
  type: oauth2
slug: nexthink-authentication
source_filename: nexthink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\ndocs: https://docs.nexthink.com/api/api-credentials\ntoken_endpoint: https://{instance}-login.{region}.nexthink.cloud/oauth2/default/v1/token\ntoken_request_auth: HTTP Basic (base64 clientId:clientSecret) on the token endpoint\ngrant_type: client_credentials\nscope: 'service:integration'\ntoken_lifetime_seconds: 900\nsource: openapi/nexthink-campaigns-api-openapi.json, openapi/nexthink-data-management-api-openapi.json,\n  openapi/nexthink-enrichment-api-openapi.json, openapi/nexthink-nql-api-openapi.json, openapi/nexthink-remote-actions-api-openapi.json,\n  openapi/nexthink-spark-api-openapi.json, openapi/nexthink-workflows-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/nexthink-campaigns-api-openapi.json\n  - openapi/nexthink-data-management-api-openapi.json\n  - openapi/nexthink-enrichment-api-openapi.json\n\
  \  - openapi/nexthink-nql-api-openapi.json\n  - openapi/nexthink-remote-actions-api-openapi.json\n  - openapi/nexthink-spark-api-openapi.json\n  - openapi/nexthink-workflows-openapi.json\n- name: publicApiAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://instance-login.region.nexthink.cloud/oauth2/default/v1/token\n    scopes: 0\n  sources:\n  - openapi/nexthink-workflows-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nexthink/refs/heads/main/authentication/nexthink-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Business Applications
- Digital Employee Experience
- Endpoint Analytics
- IT Operations
- Automation
- Observability
- DEX
---
