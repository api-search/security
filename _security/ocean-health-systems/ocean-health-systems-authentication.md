---
api_key_in:
- header
api_specs:
- filename: ocean-health-systems-ckm-rest-api-openapi.json
  format: json
  label: CKM REST API
  slug: ckm-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/openapi/ocean-health-systems-ckm-rest-api-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ocean Health Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ocean Health Systems secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ocean Health Systems
provider_slug: ocean-health-systems
scheme_count: 2
schemes:
- description: Once the session id is known, it can be used for authentication until expired. The provided session id is used (and validated) on making an actual request.
  in: header
  name: sessionid
  parameter: JSESSIONID
  sources:
  - openapi/ocean-health-systems-ckm-rest-api-openapi.json
  type: apiKey
- description: Basic authentification using the CKM username and password. The provided credentials are used (and validated) on making an actual request.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/ocean-health-systems-ckm-rest-api-openapi.json
  type: http
slug: ocean-health-systems-authentication
source_filename: ocean-health-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: derived\nsource: openapi/ocean-health-systems-ckm-rest-api-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: sessionid\n  type: apiKey\n  in: header\n  parameter: JSESSIONID\n  description: Once the session id is known, it can be used for authentication until expired.\n    The provided session id is used (and validated) on making an actual request.\n  sources:\n  - openapi/ocean-health-systems-ckm-rest-api-openapi.json\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic authentification using the CKM username and password. The provided credentials\n    are used (and validated) on making an actual request.\n  sources:\n  - openapi/ocean-health-systems-ckm-rest-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ocean-health-systems/refs/heads/main/authentication/ocean-health-systems-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Health
- Healthcare
- Electronic Health Records
- openEHR
- Clinical Data
- Clinical Knowledge Management
- Interoperability
- Health Informatics
- Terminology
- Archetypes
- Infection Prevention
- Immunisation
---
