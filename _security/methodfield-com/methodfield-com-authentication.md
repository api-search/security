---
anonymous_access: false
api_key_in: []
api_specs:
- filename: methodfield-com-admission-api-openapi.yml
  format: yaml
  label: Methodfield Admission API
  slug: methodfield-com-admission-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/methodfield-com/openapi/methodfield-com-admission-api-openapi.yml
- filename: methodfield-com-conversations-api-openapi.yml
  format: yaml
  label: Methodfield Conversations API
  slug: methodfield-com-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/methodfield-com/openapi/methodfield-com-conversations-api-openapi.yml
- filename: methodfield-com-health-api-openapi.yml
  format: yaml
  label: Methodfield Health API
  slug: methodfield-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/methodfield-com/openapi/methodfield-com-health-api-openapi.yml
- filename: methodfield-com-identity-api-openapi.yml
  format: yaml
  label: Methodfield Identity API
  slug: methodfield-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/methodfield-com/openapi/methodfield-com-identity-api-openapi.yml
- filename: methodfield-com-policy-api-openapi.yml
  format: yaml
  label: Methodfield Policy API
  slug: methodfield-com-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/methodfield-com/openapi/methodfield-com-policy-api-openapi.yml
- filename: methodfield-com-public-api-openapi.yml
  format: yaml
  label: Methodfield Public API
  slug: methodfield-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/methodfield-com/openapi/methodfield-com-public-api-openapi.yml
- filename: methodfield-com-requests-api-openapi.yml
  format: yaml
  label: Methodfield Requests API
  slug: methodfield-com-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/methodfield-com/openapi/methodfield-com-requests-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Methodfield Authentication
name_suffix: Authentication
oauth_flows: []
overview: Methodfield secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Methodfield
provider_slug: methodfield-com
scheme_count: 1
schemes:
- description: Session token issued by POST /v1/hello (bct_…, 256 bits, expires after 90 days). It authorizes exactly one conversation. Never put it in URLs or logs.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/methodfield-com-openapi.json
  type: http
slug: methodfield-com-authentication
source_filename: methodfield-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/methodfield-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Session token issued by POST /v1/hello (bct_…, 256 bits, expires after 90 days).\n    It authorizes exactly one conversation. Never put it in URLs or logs.\n  sources:\n  - openapi/methodfield-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/methodfield-com/authentication/methodfield-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- Artificial Intelligence
- Decision-Making
- Learning
---
