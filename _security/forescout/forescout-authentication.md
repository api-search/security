---
api_key_in: []
api_specs:
- filename: postman
  format: yaml
  label: Forescout Web API (Open Integration Module)
  slug: forescout-web-api-open-integration-module
  spec_type: Postman
  url: https://github.com/Forescout/examples/tree/master/web-api/postman
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Forescout Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forescout secures its APIs with http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Forescout
provider_slug: forescout
scheme_count: 4
schemes:
- api: Forescout Web API (Open Integration Module)
  flow: Obtain a session token by POSTing to /api/login with the DEX/Web API service account credentials (HTTP Basic). The response returns a JWT session token.
  login_endpoint: POST /api/login
  name: WebApiLogin
  scheme: basic
  source: https://github.com/Forescout/examples/tree/master/web-api
  type: http
- api: Forescout Web API (Open Integration Module)
  bearer_format: JWT
  flow: Pass the JWT returned by /api/login in the Authorization header on all subsequent Web API requests (e.g. GET /api/hosts, GET /api/policies, GET /api/hostfields). Tokens expire and must be refreshed via /api/login.
  header: Authorization
  name: WebApiBearer
  scheme: bearer
  source: https://github.com/Forescout/examples/tree/master/web-api/postman
  type: http
- api: Forescout eyeInspect Command Center REST API
  flow: Authenticate to the eyeInspect Command Center REST API with the Command Center username and password (HTTP Basic) over HTTPS. Access requires an eyeExtend / eyeInspect license.
  name: EyeInspectBasic
  scheme: basic
  source: https://docs.forescout.com/bundle/eyeinspect_api_guide_v5_5_0/
  type: http
- api: Forescout eyeSight Admin API
  flow: The eyeSight Admin API plugin authenticates with Forescout console credentials; see the admin-switch-api examples and Postman collection.
  name: AdminApiBasic
  scheme: basic
  source: https://github.com/Forescout/examples/tree/master/admin-switch-api
  type: http
slug: forescout-authentication
source_filename: forescout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.forescout.com/bundle/web-api-1-5-3-h/page/web-api-1-5-3-h.RESTful-Web-Service-Interaction.html\ndocs:\n- https://docs.forescout.com/bundle/web-api-1-5-3-h/\n- https://docs.forescout.com/bundle/eyeinspect_api_guide_v5_5_0/\n- https://github.com/Forescout/examples\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  - basic\n  notes: >-\n    Forescout appliances are customer-hosted, so there is no single public base\n    host; each API is reached at the customer's Enterprise Manager, eyeInspect\n    Command Center, or appliance address over HTTPS.\nschemes:\n- name: WebApiLogin\n  api: Forescout Web API (Open Integration Module)\n  type: http\n  scheme: basic\n  flow: >-\n    Obtain a session token by POSTing to /api/login with the DEX/Web API service\n    account credentials (HTTP Basic). The response returns a JWT session token.\n  login_endpoint: POST /api/login\n  source: https://github.com/Forescout/examples/tree/master/web-api\n\
  - name: WebApiBearer\n  api: Forescout Web API (Open Integration Module)\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  header: Authorization\n  flow: >-\n    Pass the JWT returned by /api/login in the Authorization header on all\n    subsequent Web API requests (e.g. GET /api/hosts, GET /api/policies,\n    GET /api/hostfields). Tokens expire and must be refreshed via /api/login.\n  source: https://github.com/Forescout/examples/tree/master/web-api/postman\n- name: EyeInspectBasic\n  api: Forescout eyeInspect Command Center REST API\n  type: http\n  scheme: basic\n  flow: >-\n    Authenticate to the eyeInspect Command Center REST API with the Command\n    Center username and password (HTTP Basic) over HTTPS. Access requires an\n    eyeExtend / eyeInspect license.\n  source: https://docs.forescout.com/bundle/eyeinspect_api_guide_v5_5_0/\n- name: AdminApiBasic\n  api: Forescout eyeSight Admin API\n  type: http\n  scheme: basic\n  flow: >-\n    The eyeSight Admin API plugin authenticates\
  \ with Forescout console\n    credentials; see the admin-switch-api examples and Postman collection.\n  source: https://github.com/Forescout/examples/tree/master/admin-switch-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forescout/refs/heads/main/authentication/forescout-authentication.yml
summary_line: http · 4 schemes
tags:
- Company
- Cybersecurity
- Network Security
- Device Visibility
- Asset Inventory
- OT Security
- IoT Security
- Vulnerability Management
- Zero Trust
- REST API
---
