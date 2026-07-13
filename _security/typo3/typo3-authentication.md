---
api_key_in: []
api_specs:
- filename: typo3-releases-openapi.json
  format: json
  label: TYPO3 Releases REST API
  slug: releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typo3/refs/heads/main/openapi/typo3-releases-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Typo3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: TYPO3 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TYPO3
provider_slug: typo3
scheme_count: 1
schemes:
- name: Basic
  scheme: basic
  sources:
  - openapi/typo3-releases-openapi.json
  type: http
slug: typo3-authentication
source_filename: typo3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/typo3-releases-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/typo3-releases-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typo3/refs/heads/main/authentication/typo3-authentication.yml
summary_line: http · 1 scheme
tags:
- CMS
- Content Management
- Enterprise
- PHP
- Headless
- JSON API
- Open Source
---
