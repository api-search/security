---
api_key_in: []
api_specs:
- filename: yardi-voyager-api-openapi.yml
  format: yaml
  label: Yardi Voyager API
  slug: yardi-voyager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi/refs/heads/main/openapi/yardi-voyager-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Yardi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yardi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Yardi
provider_slug: yardi
scheme_count: 1
schemes:
- description: SOAP authentication using UserName, Password, and ServerName parameters passed within the SOAP request body. Credentials are provided by the Yardi Standard Interface Partnership Program.
  name: soapAuth
  scheme: basic
  sources:
  - openapi/yardi-voyager-api-openapi.yml
  type: http
slug: yardi-authentication
source_filename: yardi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/yardi-voyager-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: soapAuth\n  type: http\n  scheme: basic\n  description: SOAP authentication using UserName, Password, and ServerName parameters passed\n    within the SOAP request body. Credentials are provided by the Yardi Standard Interface Partnership\n    Program.\n  sources:\n  - openapi/yardi-voyager-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yardi/refs/heads/main/authentication/yardi-authentication.yml
summary_line: http · 1 scheme
tags:
- Accounting
- Commercial Real Estate
- Coworking
- Investment Management
- Multifamily
- Property Management
- Real Estate
- Residential
- Self Storage
- Senior Living
---
