---
api_key_in: []
api_specs:
- filename: oracle-otm-business-objects-openapi.yml
  format: yaml
  label: Oracle Transportation Management Business Object Resources REST API
  slug: oracle-transportation-management-business-object-resources-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-transportation-management/refs/heads/main/openapi/oracle-otm-business-objects-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Transportation Management Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Oracle Transportation Management secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Oracle Transportation Management
provider_slug: oracle-transportation-management
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://login.oracle.com/oauth2/v1/token
  name: oauth2
  sources:
  - openapi/oracle-otm-business-objects-openapi.yml
  type: oauth2
slug: oracle-transportation-management-authentication
source_filename: oracle-transportation-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-otm-business-objects-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.oracle.com/oauth2/v1/token\n    scopes: 2\n  sources:\n  - openapi/oracle-otm-business-objects-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-transportation-management/refs/heads/main/authentication/oracle-transportation-management-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Logistics
- Transportation
- Freight
- Supply Chain
- Shipping
- Global Trade
- Oracle
---
