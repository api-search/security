---
anonymous_access: false
api_key_in: []
api_specs:
- filename: axiomatics-authorize-api-openapi.yml
  format: yaml
  label: Axiomatics Authorize API
  slug: axiomatics-authorize-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiomatics/openapi/axiomatics-authorize-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Axiomatics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Axiomatics secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Axiomatics
provider_slug: axiomatics
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/axiomatics-xacml.yaml
  type: http
slug: axiomatics-authentication
source_filename: axiomatics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/axiomatics-xacml.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/axiomatics-xacml.yaml\n"
source_yaml_url: https://artifacts.apis.io/axiomatics/authentication/axiomatics-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Authorization
- Policy
- ZeroTrust
- Compliance
- Enterprise
---
