---
anonymous_access: false
api_key_in: []
api_specs:
- filename: appen-download-api-openapi.yml
  format: yaml
  label: Appen Download API
  slug: appen-download-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-download-api-openapi.yml
- filename: appen-internal-contributors-api-openapi.yml
  format: yaml
  label: Appen Internal Contributors API
  slug: appen-internal-contributors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-internal-contributors-api-openapi.yml
- filename: appen-jobs-api-openapi.yml
  format: yaml
  label: Appen Jobs API
  slug: appen-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-jobs-api-openapi.yml
- filename: appen-projects-api-openapi.yml
  format: yaml
  label: Appen Projects API
  slug: appen-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-projects-api-openapi.yml
- filename: appen-route-units-api-openapi.yml
  format: yaml
  label: Appen Route Units API
  slug: appen-route-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-route-units-api-openapi.yml
- filename: appen-test-questions-api-openapi.yml
  format: yaml
  label: Appen Test Questions API
  slug: appen-test-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-test-questions-api-openapi.yml
- filename: appen-upload-api-openapi.yml
  format: yaml
  label: Appen Upload API
  slug: appen-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/openapi/appen-upload-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Appen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appen secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Appen
provider_slug: appen
scheme_count: 1
schemes:
- bearerFormat: Token
  description: 'API Token authentication. Pass your API token in the Authorization header:

    `Authorization: Token token=your-api-token-here`'
  name: TokenAuth
  scheme: bearer
  sources:
  - openapi/appen-openapi-remote.yaml
  type: http
slug: appen-authentication
source_filename: appen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: derived\nsource: openapi/appen-openapi-remote.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: TokenAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Token\n  description: |-\n    API Token authentication. Pass your API token in the Authorization header:\n    `Authorization: Token token=your-api-token-here`\n  sources:\n  - openapi/appen-openapi-remote.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appen/refs/heads/main/authentication/appen-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Data
- Annotation
- TrainingData
- Enterprise
---
