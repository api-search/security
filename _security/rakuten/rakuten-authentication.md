---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Rakuten Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rakuten secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rakuten
provider_slug: rakuten
scheme_count: 2
schemes:
- description: Rakuten application ID (issued from the RWS developer console).
  in: query
  name: applicationId
  parameter: applicationId
  sources:
  - openapi/rakuten-openapi.yml
  type: apiKey
- description: Rakuten RWS access key. May also be supplied as an HTTP header.
  in: query
  name: accessKey
  parameter: accessKey
  sources:
  - openapi/rakuten-openapi.yml
  type: apiKey
slug: rakuten-authentication
source_filename: rakuten-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rakuten-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: applicationId\n  type: apiKey\n  in: query\n  parameter: applicationId\n  description: Rakuten application ID (issued from the RWS developer console).\n  sources:\n  - openapi/rakuten-openapi.yml\n- name: accessKey\n  type: apiKey\n  in: query\n  parameter: accessKey\n  description: Rakuten RWS access key. May also be supplied as an HTTP header.\n  sources:\n  - openapi/rakuten-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rakuten/refs/heads/main/authentication/rakuten-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- E-commerce
- Travel
- Books
- Recipes
- Golf
- Japan
- Fintech
- Telecom
- Rakuten Web Services
---
