---
api_key_in:
- header
- url-userinfo
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Splunk Soar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Splunk SOAR secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Splunk SOAR
provider_slug: splunk-soar
scheme_count: 2
schemes:
- description: HTTP Basic authentication with a SOAR username and password. Required (token auth is not accepted) for DELETE operations.
  example: curl -u "username:password" https://{soar-host}/rest/container/1
  name: basicAuth
  scheme: basic
  source: docs
  type: http
- constraints:
  - Cannot be used for DELETE requests — those require user-account (basic) authentication.
  description: 'Automation-user authorization token. Created per automation (service) user in the SOAR admin interface; the interface returns a JSON blob containing the ph-auth-token value and the server URL. Can also be supplied as the password half of the URL userinfo: https://:<token>@{soar-host}/rest/container/1'
  in: header
  name: phAuthToken
  name_param: ph-auth-token
  source: docs
  type: apiKey
slug: splunk-soar-authentication
source_filename: splunk-soar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: https://help.splunk.com/en/splunk-soar/soar-cloud/rest-api-reference/using-the-splunk-soar-rest-api/using-the-rest-api-reference-for-splunk-soar-cloud\ndocs: https://help.splunk.com/en/splunk-soar/soar-cloud/rest-api-reference/using-the-splunk-soar-rest-api/using-the-rest-api-reference-for-splunk-soar-cloud\nnote: >-\n  Derived from the published Splunk SOAR REST API reference, not from an OpenAPI document — Splunk\n  publishes no anonymously fetchable machine-readable contract for SOAR (see apis.yml\n  x-contract-status). No OAuth 2.0 or OpenID Connect surface is documented for the SOAR REST API.\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  - url-userinfo\n  oauth2_flows: []\n  transport: https-required\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication with a SOAR username and password. Required (token auth is not\n    accepted) for DELETE\
  \ operations.\n  example: curl -u \"username:password\" https://{soar-host}/rest/container/1\n  source: docs\n- name: phAuthToken\n  type: apiKey\n  in: header\n  name_param: ph-auth-token\n  description: >-\n    Automation-user authorization token. Created per automation (service) user in the SOAR admin\n    interface; the interface returns a JSON blob containing the ph-auth-token value and the server\n    URL. Can also be supplied as the password half of the URL userinfo:\n    https://:<token>@{soar-host}/rest/container/1\n  source: docs\n  constraints:\n  - Cannot be used for DELETE requests — those require user-account (basic) authentication.\ntransport:\n  https_required: true\n  statement: >-\n    \"REST API requests must be performed over HTTPS, and only authorized users and devices are allowed.\"\nauthorization:\n  model: role-based\n  note: >-\n    SOAR enforces role-based access control on top of authentication; roles and permissions are\n    managed through the role-management\
  \ endpoints\n    (https://help.splunk.com/en/splunk-soar/soar-cloud/rest-api-reference/role-management-endpoints).\n  scopes: none-documented\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/splunk-soar/refs/heads/main/authentication/splunk-soar-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Security
- SOAR
- Automation
- Orchestration
- Incident Response
- SOC
- Security Operations
- Playbooks
- Case Management
- Threat Intelligence
---
