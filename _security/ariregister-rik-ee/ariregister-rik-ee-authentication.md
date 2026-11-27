---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ariregister-rik-ee-beneficialowners-api-openapi.yml
  format: yaml
  label: Estonian e-Business Register (RIK) Beneficial Owners API
  slug: ariregister-rik-ee-beneficialowners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ariregister-rik-ee/openapi/ariregister-rik-ee-beneficialowners-api-openapi.yml
- filename: ariregister-rik-ee-company-api-openapi.yml
  format: yaml
  label: Estonian e-Business Register (RIK) Company API
  slug: ariregister-rik-ee-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ariregister-rik-ee/openapi/ariregister-rik-ee-company-api-openapi.yml
- filename: ariregister-rik-ee-keylogin-api-openapi.yml
  format: yaml
  label: Estonian e-Business Register (RIK) Key Login API
  slug: ariregister-rik-ee-keylogin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ariregister-rik-ee/openapi/ariregister-rik-ee-keylogin-api-openapi.yml
- filename: ariregister-rik-ee-person-api-openapi.yml
  format: yaml
  label: Estonian e-Business Register (RIK) Person API
  slug: ariregister-rik-ee-person-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ariregister-rik-ee/openapi/ariregister-rik-ee-person-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Estonian e-Business Register (RIK) Authentication
name_suffix: Authentication
oauth_flows: []
overview: Estonian e-Business Register (RIK) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Estonian e-Business Register (RIK)
provider_slug: ariregister-rik-ee
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: OAuth2PasswordBearer
  scheme: bearer
  sources:
  - openapi/ariregister-rik-ee-openapi.yml
  type: http
slug: ariregister-rik-ee-authentication
source_filename: ariregister-rik-ee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/ariregister-rik-ee-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: OAuth2PasswordBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/ariregister-rik-ee-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/ariregister-rik-ee/authentication/ariregister-rik-ee-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Government
- Business Registry
- Open Data
- Estonia
- Beneficial Ownership
- SOAP
- KYB
---
