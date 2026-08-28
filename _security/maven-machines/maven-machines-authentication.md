---
api_key_in:
- header
api_specs:
- filename: maven-machines-users-openapi.json
  format: json
  label: Maven Integrations API
  slug: maven-machines-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-machines/refs/heads/main/openapi/maven-machines-users-openapi.json
- filename: maven-machines-aaa-cooper-middleware-openapi.json
  format: json
  label: Maven Customer Integration Middleware
  slug: maven-machines-customer-middleware
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maven-machines/refs/heads/main/openapi/maven-machines-aaa-cooper-middleware-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Maven Machines Authentication
name_suffix: Authentication
oauth_flows: []
overview: Maven Machines secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Maven Machines
provider_slug: maven-machines
scheme_count: 1
schemes:
- description: 'A single per-fleet, per-environment key sent as the `apiKey` request header on every protected call. Maven states it plainly in the middleware documentation: "All protected endpoints require an API key in the `apiKey` request header", and "Your `apiKey` determines which Maven environment (dev, qa, staging, prod) receives the request." The truckload documentation adds that "the apiKey header authenticates and authorizes the request to submit trip data for a specific company" — so the key is the tenant selector as well as the credential.'
  in: header
  name: api_key
  parameter: apiKey
  sources:
  - openapi/maven-machines-users-openapi.json
  - openapi/maven-machines-assets-openapi.json
  - openapi/maven-machines-company-locations-openapi.json
  - openapi/maven-machines-shipments-openapi.json
  - openapi/maven-machines-shipment-locations-openapi.json
  - openapi/maven-machines-linehaul-openapi.json
  - openapi/maven-machines-manifest-commands-openapi.json
  - openapi/maven-machines-planning-and-dispatch-openapi.json
  - openapi/maven-machines-workflow-openapi.json
  - openapi/maven-machines-messages-openapi.json
  - openapi/maven-machines-market-apps-openapi.json
  - openapi/maven-machines-smart-openapi.json
  - openapi/maven-machines-reports-openapi.json
  - openapi/maven-machines-rest-service-manual-openapi.json
  - openapi/maven-machines-aaa-cooper-middleware-openapi.json
  - openapi/maven-machines-averitt-middleware-openapi.json
  - openapi/maven-machines-bozzutos-middleware-openapi.json
  - openapi/maven-machines-reddy-ice-middleware-openapi.json
  - openapi/maven-machines-roy-miller-middleware-openapi.json
  - openapi/maven-machines-triple-s-steel-middleware-openapi.json
  type: apiKey
slug: maven-machines-authentication
source_filename: maven-machines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: >-\n  https://maven-machines.readme.io/docs/basic-concepts.md and\n  https://maven-machines.readme.io/docs/standard-tms-integration.md (docs), reconciled against the\n  securitySchemes declared in all 21 documents under openapi/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  http_basic: false\n  http_bearer: false\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: >-\n    A single per-fleet, per-environment key sent as the `apiKey` request header on every protected\n    call. Maven states it plainly in the middleware documentation: \"All protected endpoints require\n    an API key in the `apiKey` request header\", and \"Your `apiKey` determines which Maven\n    environment (dev, qa, staging, prod) receives the request.\" The truckload documentation adds\n    that \"the apiKey header authenticates and authorizes\
  \ the request to submit trip data for a\n    specific company\" — so the key is the tenant selector as well as the credential.\n  sources:\n  - openapi/maven-machines-users-openapi.json\n  - openapi/maven-machines-assets-openapi.json\n  - openapi/maven-machines-company-locations-openapi.json\n  - openapi/maven-machines-shipments-openapi.json\n  - openapi/maven-machines-shipment-locations-openapi.json\n  - openapi/maven-machines-linehaul-openapi.json\n  - openapi/maven-machines-manifest-commands-openapi.json\n  - openapi/maven-machines-planning-and-dispatch-openapi.json\n  - openapi/maven-machines-workflow-openapi.json\n  - openapi/maven-machines-messages-openapi.json\n  - openapi/maven-machines-market-apps-openapi.json\n  - openapi/maven-machines-smart-openapi.json\n  - openapi/maven-machines-reports-openapi.json\n  - openapi/maven-machines-rest-service-manual-openapi.json\n  - openapi/maven-machines-aaa-cooper-middleware-openapi.json\n  - openapi/maven-machines-averitt-middleware-openapi.json\n\
  \  - openapi/maven-machines-bozzutos-middleware-openapi.json\n  - openapi/maven-machines-reddy-ice-middleware-openapi.json\n  - openapi/maven-machines-roy-miller-middleware-openapi.json\n  - openapi/maven-machines-triple-s-steel-middleware-openapi.json\ntenancy:\n  model: key-scoped\n  detail: >-\n    The key binds a caller to one company. A 401 in the users specification is described as \"This\n    endpoint may only be executed for company 1\". The planning-and-dispatch definition additionally\n    templates the tenant into the server URL —\n    https://integrations.mavenmachines.com/companies/{companyKey}/ — so a caller integrating\n    against that definition supplies the company twice, once in the path and once implicitly\n    through the key.\nenvironments:\n- name: production\n  base_url: https://integrations.mavenmachines.com/\n- name: staging\n  base_url: https://integrations-staging.mavenmachines.com/\n  note: Keys are not interchangeable between environments.\nkey_management:\n\
  \  self_serve: false\n  rotation_documented: false\n  scopes: false\n  expiry_documented: false\n  detail: >-\n    Maven publishes no key-issuance, rotation, expiry or revocation procedure, no scope or\n    permission model on the key, and no self-serve developer signup. Keys are provisioned to\n    contracted fleets. Driver-facing permissions (e.g. \"Market App Access\") are managed in the Maven\n    Fleet Admin portal as user roles, not as API scopes.\npublic_endpoints:\n- path: GET /\n  service: reddy-ice middleware\n  detail: '\"GET / is public and does not require an API key.\" Health check only; returns \"Hello World!\".'\ngaps:\n- >-\n  All 17 OpenAPI 3.0.0 documents DECLARE the apiKey scheme in components.securitySchemes but do NOT\n  apply it at document level (`security` is null). Only the four 3.1.0 documents carry a top-level\n  security requirement. A client generated from the 3.0.0 documents authenticates nothing by\n  default — see overlays/ for the correction.\n- No OAuth,\
  \ OIDC or mTLS option for enterprise fleets; a single long-lived shared header key is the\n  only credential.\n- /.well-known/openid-configuration and /.well-known/oauth-authorization-server return 404 on every\n  Maven host, including accounts.mavenmachines.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maven-machines/refs/heads/main/authentication/maven-machines-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Transportation
- Logistics
- Trucking
- Fleet Management
- Telematics
- ELD
- Route Optimization
- Dispatch
- Supply Chain
- Freight
---
