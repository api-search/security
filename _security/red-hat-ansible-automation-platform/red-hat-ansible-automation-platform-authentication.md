---
api_key_in:
- cookie
- header
api_specs:
- filename: red-hat-ansible-automation-platform-automation-controller-openapi.json
  format: json
  label: Red Hat Ansible Automation Controller API
  slug: controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/openapi/red-hat-ansible-automation-platform-automation-controller-openapi.json
- filename: red-hat-ansible-automation-platform-automation-hub-openapi.json
  format: json
  label: Red Hat Ansible Private Automation Hub API
  slug: private-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/openapi/red-hat-ansible-automation-platform-automation-hub-openapi.json
- filename: red-hat-ansible-automation-platform-event-driven-ansible-openapi.json
  format: json
  label: Red Hat Event-Driven Ansible Controller API
  slug: eda-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/openapi/red-hat-ansible-automation-platform-event-driven-ansible-openapi.json
- filename: red-hat-ansible-automation-platform-platform-gateway-openapi.json
  format: json
  label: Red Hat Ansible Automation Platform Gateway API
  slug: platform-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json
- filename: red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json
  format: json
  label: Red Hat Ansible Lightspeed with IBM watsonx Code Assistant API
  slug: ansible-lightspeed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json
- filename: red-hat-ansible-automation-platform-automation-hub-openapi.json
  format: json
  label: Red Hat Automation Hub API (Hybrid Cloud Console)
  slug: hosted-automation-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/openapi/red-hat-ansible-automation-platform-automation-hub-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Red Hat Ansible Automation Platform Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: Red Hat Ansible Automation Platform secures its APIs with apiKey, http, and oauth2 across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: Red Hat Ansible Automation Platform
provider_slug: red-hat-ansible-automation-platform
scheme_count: 6
schemes:
- in: cookie
  name: cookieAuth
  parameter: sessionid
  sources:
  - openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json
  - openapi/red-hat-ansible-automation-platform-event-driven-ansible-openapi.json
  type: apiKey
- flows:
  - authorizationUrl: /o/authorize/
    flow: authorizationCode
    scopes: 3
    tokenUrl: /o/token/
  name: oauth2
  sources:
  - openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json
  type: oauth2
- in: header
  name: EDAJWTAuthentication
  parameter: X-DAB-JW-TOKEN
  sources:
  - openapi/red-hat-ansible-automation-platform-event-driven-ansible-openapi.json
  type: apiKey
- name: Basic_Authentication
  scheme: basic
  sources:
  - openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json
  type: http
- flows:
  - authorizationUrl: /o/authorize/
    flow: authorizationCode
    scopes: 2
    tokenUrl: /o/token/
  - flow: password
    scopes: 2
    tokenUrl: /o/token/
  name: OAuth2_Authentication
  sources:
  - openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json
  type: oauth2
- in: cookie
  name: SessionAuthentication
  parameter: gateway_sessionid
  sources:
  - openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json
  type: apiKey
slug: red-hat-ansible-automation-platform-authentication
source_filename: red-hat-ansible-automation-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: derived\nsource: openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json, openapi/red-hat-ansible-automation-platform-event-driven-ansible-openapi.json,\n  openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - password\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  sources:\n  - openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json\n  - openapi/red-hat-ansible-automation-platform-event-driven-ansible-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /o/authorize/\n    tokenUrl: /o/token/\n    scopes: 3\n  sources:\n  - openapi/red-hat-ansible-automation-platform-ansible-lightspeed-openapi.json\n- name: EDAJWTAuthentication\n  type: apiKey\n  in: header\n\
  \  parameter: X-DAB-JW-TOKEN\n  sources:\n  - openapi/red-hat-ansible-automation-platform-event-driven-ansible-openapi.json\n- name: Basic_Authentication\n  type: http\n  scheme: basic\n  sources:\n  - openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json\n- name: OAuth2_Authentication\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /o/authorize/\n    tokenUrl: /o/token/\n    scopes: 2\n  - flow: password\n    tokenUrl: /o/token/\n    scopes: 2\n  sources:\n  - openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json\n- name: SessionAuthentication\n  type: apiKey\n  in: cookie\n  parameter: gateway_sessionid\n  sources:\n  - openapi/red-hat-ansible-automation-platform-platform-gateway-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-ansible-automation-platform/refs/heads/main/authentication/red-hat-ansible-automation-platform-authentication.yml
summary_line: apiKey/http/oauth2 · 6 schemes
tags:
- Automation
- Configuration Management
- DevOps
- Enterprise
- Red Hat
- Ansible
- IT Operations
- Event-Driven Architecture
- Infrastructure as Code
- MCP
---
