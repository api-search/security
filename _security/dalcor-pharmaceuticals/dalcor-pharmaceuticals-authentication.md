---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Dalcor Pharmaceuticals Authentication
name_suffix: Authentication
oauth_flows: []
overview: DalCor Pharmaceuticals secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DalCor Pharmaceuticals
provider_slug: dalcor-pharmaceuticals
scheme_count: 1
schemes:
- description: WordPress Application Passwords (RFC 7617 Basic over TLS). Required only for write and administrative routes, which are out of scope for this document — every operation modelled here returns 200 anonymously.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/dalcor-pharmaceuticals-content-openapi.yml
  type: http
slug: dalcor-pharmaceuticals-authentication
source_filename: dalcor-pharmaceuticals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/dalcor-pharmaceuticals-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (RFC 7617 Basic over TLS). Required only for\n    write and administrative routes, which are out of scope for this document — every operation\n    modelled here returns 200 anonymously.\n  sources:\n  - openapi/dalcor-pharmaceuticals-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dalcor-pharmaceuticals/refs/heads/main/authentication/dalcor-pharmaceuticals-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Pharmaceuticals
- Biotechnology
- Cardiovascular
- Precision Medicine
- Pharmacogenomics
- Clinical Trials
- Life Sciences
- content-api
---
