---
api_key_in: []
api_specs:
- filename: datto-rmm-openapi.json
  format: json
  label: Datto RMM API
  slug: datto-rmm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datto/refs/heads/main/openapi/datto-rmm-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Datto Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Datto secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Datto
provider_slug: datto
scheme_count: 1
schemes:
- bearer_format: JWT access token
  flow: password
  name: OAuth2
  presented_as: Authorization Bearer
  regional_hosts:
  - concord-api.centrastage.net
  - merlot-api.centrastage.net
  - pinotage-api.centrastage.net
  - vidal-api.centrastage.net
  - zinfandel-api.centrastage.net
  - syrah-api.centrastage.net
  sources:
  - openapi/datto-rmm-openapi.json
  token_endpoint: https://[platform]-api.centrastage.net/auth/oauth/token
  token_ttl_hours: 100
  type: oauth2
slug: datto-authentication
source_filename: datto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://rmm.datto.com/help/en/Content/2SETUP/APIv2.htm\ndocs: https://rmm.datto.com/help/en/Content/2SETUP/APIv2.htm\nnote: >-\n  The Datto RMM v2 OpenAPI does not declare securitySchemes in components, but\n  the API v2 documentation specifies OAuth 2.0. A user generates an API Key and\n  API Secret Key in the RMM Setup interface; those credentials are exchanged for\n  an OAuth 2.0 access token which is presented as a Bearer token on subsequent\n  requests. Access tokens expire after 100 hours. Requests are scoped to the\n  permissions of the RMM user whose keys were used.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\n  token_lifetime: 100 hours\n  credential_source: API Key + API Secret Key generated in RMM Setup\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: password\n  token_endpoint: https://[platform]-api.centrastage.net/auth/oauth/token\n  presented_as: Authorization Bearer\n  bearer_format: JWT\
  \ access token\n  token_ttl_hours: 100\n  regional_hosts:\n  - concord-api.centrastage.net\n  - merlot-api.centrastage.net\n  - pinotage-api.centrastage.net\n  - vidal-api.centrastage.net\n  - zinfandel-api.centrastage.net\n  - syrah-api.centrastage.net\n  sources:\n  - openapi/datto-rmm-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datto/refs/heads/main/authentication/datto-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Data Protection
- Backup
- Disaster Recovery
- Managed Service Providers
- Remote Monitoring and Management
- Endpoint Management
- Cybersecurity
- IT Operations
- SaaS Protection
---
