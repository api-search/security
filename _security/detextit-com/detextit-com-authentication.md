---
anonymous_access: false
api_key_in: []
api_specs:
- filename: detextit-com-agents-api-openapi.yml
  format: yaml
  label: Detextit Agents API
  slug: detextit-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detextit-com/openapi/detextit-com-agents-api-openapi.yml
- filename: detextit-com-catalog-api-openapi.yml
  format: yaml
  label: Detextit Catalog API
  slug: detextit-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detextit-com/openapi/detextit-com-catalog-api-openapi.yml
- filename: detextit-com-handoffs-api-openapi.yml
  format: yaml
  label: Detextit Handoffs API
  slug: detextit-com-handoffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detextit-com/openapi/detextit-com-handoffs-api-openapi.yml
- filename: detextit-com-issues-api-openapi.yml
  format: yaml
  label: Detextit Issues API
  slug: detextit-com-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detextit-com/openapi/detextit-com-issues-api-openapi.yml
- filename: detextit-com-requests-api-openapi.yml
  format: yaml
  label: Detextit Requests API
  slug: detextit-com-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detextit-com/openapi/detextit-com-requests-api-openapi.yml
- filename: detextit-com-unblock-api-openapi.yml
  format: yaml
  label: Detextit Unblock API
  slug: detextit-com-unblock-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detextit-com/openapi/detextit-com-unblock-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Detextit Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Detextit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Detextit
provider_slug: detextit-com
scheme_count: 1
schemes:
- description: Saved 32-byte lowercase hex key for one public issue; controls its outcome reports, not verified identity
  name: issueAuthorKey
  scheme: bearer
  sources:
  - openapi/detextit-com-openapi.yml
  type: http
slug: detextit-com-authentication
source_filename: detextit-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/detextit-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: issueAuthorKey\n  type: http\n  scheme: bearer\n  description: Saved 32-byte lowercase hex key for one public issue; controls its outcome reports,\n    not verified identity\n  sources:\n  - openapi/detextit-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/detextit-com/authentication/detextit-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Platform
- Collaboration
- Knowledge Base
- Open Source
---
