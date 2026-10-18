---
anonymous_access: false
api_key_in: []
api_specs:
- filename: internet2-co-api-openapi.yml
  format: yaml
  label: Internet2 Co API
  slug: internet2-co-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-api-openapi.yml
- filename: internet2-co-group-members-api-openapi.yml
  format: yaml
  label: Internet2 Co Group Members API
  slug: internet2-co-group-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-group-members-api-openapi.yml
- filename: internet2-co-group-members-json-api-openapi.yml
  format: yaml
  label: Internet2 Co Group Members.json API
  slug: internet2-co-group-members-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-group-members-json-api-openapi.yml
- filename: internet2-co-groups-api-openapi.yml
  format: yaml
  label: Internet2 Co Groups API
  slug: internet2-co-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-groups-api-openapi.yml
- filename: internet2-co-groups-json-api-openapi.yml
  format: yaml
  label: Internet2 Co Groups.json API
  slug: internet2-co-groups-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-groups-json-api-openapi.yml
- filename: internet2-co-people-api-openapi.yml
  format: yaml
  label: Internet2 Co People API
  slug: internet2-co-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-people-api-openapi.yml
- filename: internet2-co-people-json-api-openapi.yml
  format: yaml
  label: Internet2 Co People.json API
  slug: internet2-co-people-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-co-people-json-api-openapi.yml
- filename: internet2-email-addresses-json-api-openapi.yml
  format: yaml
  label: Internet2 Email Addresses.json API
  slug: internet2-email-addresses-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/openapi/internet2-email-addresses-json-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Internet2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Internet2 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Internet2
provider_slug: internet2
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/comanage-registry-restapiv1.yml
  type: http
slug: internet2-authentication
source_filename: internet2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: derived\nsource: openapi/comanage-registry-restapiv1.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/comanage-registry-restapiv1.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/internet2/refs/heads/main/authentication/internet2-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Networking
- Research
- Education
- Non-Profit
---
