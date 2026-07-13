---
api_key_in:
- header
api_specs:
- filename: cwaf-v1-swagger-3.json
  format: json
  label: Imperva Cloud Application Security API
  slug: cloud-application-security-api
  spec_type: OpenAPI
  url: https://github.com/imperva/imperva-web-api-composer/blob/master/src/assets/cwaf/cwaf-v1-swagger-3.json
- filename: securesphere-swagger
  format: yaml
  label: Imperva SecureSphere Open API
  slug: securesphere-open-api
  spec_type: OpenAPI
  url: https://github.com/imperva-dev/securesphere-swagger
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Imperva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Imperva secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Imperva
provider_slug: imperva
scheme_count: 3
schemes:
- in: header
  name: api_id
  parameter: x-API-Id
  sources:
  - openapi/imperva-cloud-application-security-openapi.yml
  type: apiKey
- in: header
  name: api_key
  parameter: x-API-Key
  sources:
  - openapi/imperva-cloud-application-security-openapi.yml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/imperva-securesphere-openapi.yml
  type: http
slug: imperva-authentication
source_filename: imperva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/imperva-cloud-application-security-openapi.yml, openapi/imperva-securesphere-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: api_id\n  type: apiKey\n  in: header\n  parameter: x-API-Id\n  sources:\n  - openapi/imperva-cloud-application-security-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-API-Key\n  sources:\n  - openapi/imperva-cloud-application-security-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/imperva-securesphere-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/authentication/imperva-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Security
- Cybersecurity
- WAF
- DDoS Protection
- API Security
- Bot Management
- Data Security
- Cloud Security
---
