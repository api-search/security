---
api_key_in:
- header
api_specs:
- filename: nhost-authentication-api-openapi.yml
  format: yaml
  label: Nhost authentication API
  slug: nhost-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-authentication-api-openapi.yml
- filename: nhost-documentation-api-openapi.yml
  format: yaml
  label: Nhost documentation API
  slug: nhost-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-documentation-api-openapi.yml
- filename: nhost-excludeme-api-openapi.yml
  format: yaml
  label: Nhost excludeme API
  slug: nhost-excludeme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-excludeme-api-openapi.yml
- filename: nhost-files-api-openapi.yml
  format: yaml
  label: Nhost files API
  slug: nhost-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-files-api-openapi.yml
- filename: nhost-operations-api-openapi.yml
  format: yaml
  label: Nhost operations API
  slug: nhost-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-operations-api-openapi.yml
- filename: nhost-security-api-openapi.yml
  format: yaml
  label: Nhost security API
  slug: nhost-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-security-api-openapi.yml
- filename: nhost-session-api-openapi.yml
  format: yaml
  label: Nhost session API
  slug: nhost-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-session-api-openapi.yml
- filename: nhost-storage-api-openapi.yml
  format: yaml
  label: Nhost storage API
  slug: nhost-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-storage-api-openapi.yml
- filename: nhost-system-api-openapi.yml
  format: yaml
  label: Nhost system API
  slug: nhost-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-system-api-openapi.yml
- filename: nhost-user-api-openapi.yml
  format: yaml
  label: Nhost user API
  slug: nhost-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-user-api-openapi.yml
- filename: nhost-verification-api-openapi.yml
  format: yaml
  label: Nhost verification API
  slug: nhost-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/openapi/nhost-verification-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nhost Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nhost secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nhost
provider_slug: nhost
scheme_count: 2
schemes:
- description: Bearer authentication with JWT access token. Used to authenticate requests to protected endpoints.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nhost-authentication-openapi.yml
  - openapi/nhost-storage-openapi.yml
  type: http
- description: Hasura admin secret key for backend/administrative operations.
  in: header
  name: X-Hasura-Admin-Secret
  parameter: X-Hasura-Admin-Secret
  sources:
  - openapi/nhost-storage-openapi.yml
  type: apiKey
slug: nhost-authentication
source_filename: nhost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nhost-authentication-openapi.yml, openapi/nhost-storage-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer authentication with JWT access token. Used to authenticate requests to\n    protected endpoints.\n  sources:\n  - openapi/nhost-authentication-openapi.yml\n  - openapi/nhost-storage-openapi.yml\n- name: X-Hasura-Admin-Secret\n  type: apiKey\n  in: header\n  parameter: X-Hasura-Admin-Secret\n  description: Hasura admin secret key for backend/administrative operations.\n  sources:\n  - openapi/nhost-storage-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhost/refs/heads/main/authentication/nhost-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- GraphQL
- PostgreSQL
- Authentication
- File Storage
- Serverless Functions
- Real-Time
- Open-Source
- Firebase Alternative
- Backend as a Service
- BaaS
---
