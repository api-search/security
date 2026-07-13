---
api_key_in:
- query
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Depositphotos Partner API
  slug: depositphotos-partner-api
  spec_type: OpenAPI
  url: https://api.depositphotos.com/doc/
- filename: depositphotos-enterprise-api.json
  format: json
  label: Depositphotos Enterprise API
  slug: depositphotos-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/depositphotos/refs/heads/main/openapi/depositphotos-enterprise-api.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Depositphotos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Depositphotos secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Depositphotos
provider_slug: depositphotos
scheme_count: 2
schemes:
- description: API key issued to the registered corporate client
  in: query
  name: ApiKeyParam
  parameter: dp_apikey
  sources:
  - openapi/depositphotos-enterprise-api.json
  - openapi/depositphotos-partner-api.json
  type: apiKey
- description: Session identifier obtained from loginEnterprise, valid for 3 hours
  in: query
  name: SessionId
  parameter: dp_session_id
  sources:
  - openapi/depositphotos-enterprise-api.json
  - openapi/depositphotos-partner-api.json
  type: apiKey
slug: depositphotos-authentication
source_filename: depositphotos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/depositphotos-enterprise-api.json, openapi/depositphotos-partner-api.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyParam\n  type: apiKey\n  in: query\n  parameter: dp_apikey\n  description: API key issued to the registered corporate client\n  sources:\n  - openapi/depositphotos-enterprise-api.json\n  - openapi/depositphotos-partner-api.json\n- name: SessionId\n  type: apiKey\n  in: query\n  parameter: dp_session_id\n  description: Session identifier obtained from loginEnterprise, valid for 3 hours\n  sources:\n  - openapi/depositphotos-enterprise-api.json\n  - openapi/depositphotos-partner-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/depositphotos/refs/heads/main/authentication/depositphotos-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Stock Photos
- Images
- Videos
- Vectors
- Media
- Creative Assets
- Generative AI
---
