---
api_key_in:
- header
api_specs:
- filename: doc.json
  format: json
  label: ISBNdb API
  slug: isbndb-api
  spec_type: OpenAPI
  url: https://api2.isbndb.com/doc.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Isbndb Authentication
name_suffix: Authentication
oauth_flows: []
overview: ISBNdb secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ISBNdb
provider_slug: isbndb
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/openapi.json
  type: apiKey
slug: isbndb-authentication
source_filename: isbndb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isbndb/refs/heads/main/authentication/isbndb-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Books
- ISBN
- Publishing
- Metadata
- Library
- Bibliography
---
