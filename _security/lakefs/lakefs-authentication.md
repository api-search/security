---
api_key_in:
- cookie
api_specs:
- filename: lakefs-actions-api-openapi.yml
  format: yaml
  label: lakeFS actions API
  slug: lakefs-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-actions-api-openapi.yml
- filename: lakefs-auth-api-openapi.yml
  format: yaml
  label: lakeFS auth API
  slug: lakefs-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-auth-api-openapi.yml
- filename: lakefs-branches-api-openapi.yml
  format: yaml
  label: lakeFS branches API
  slug: lakefs-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-branches-api-openapi.yml
- filename: lakefs-commits-api-openapi.yml
  format: yaml
  label: lakeFS commits API
  slug: lakefs-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-commits-api-openapi.yml
- filename: lakefs-config-api-openapi.yml
  format: yaml
  label: lakeFS config API
  slug: lakefs-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-config-api-openapi.yml
- filename: lakefs-experimental-api-openapi.yml
  format: yaml
  label: lakeFS experimental API
  slug: lakefs-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-experimental-api-openapi.yml
- filename: lakefs-external-api-openapi.yml
  format: yaml
  label: lakeFS external API
  slug: lakefs-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-external-api-openapi.yml
- filename: lakefs-healthcheck-api-openapi.yml
  format: yaml
  label: lakeFS healthCheck API
  slug: lakefs-healthcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-healthcheck-api-openapi.yml
- filename: lakefs-import-api-openapi.yml
  format: yaml
  label: lakeFS import API
  slug: lakefs-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-import-api-openapi.yml
- filename: lakefs-internal-api-openapi.yml
  format: yaml
  label: lakeFS internal API
  slug: lakefs-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-internal-api-openapi.yml
- filename: lakefs-metadata-api-openapi.yml
  format: yaml
  label: lakeFS metadata API
  slug: lakefs-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-metadata-api-openapi.yml
- filename: lakefs-objects-api-openapi.yml
  format: yaml
  label: lakeFS objects API
  slug: lakefs-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-objects-api-openapi.yml
- filename: lakefs-pulls-api-openapi.yml
  format: yaml
  label: lakeFS pulls API
  slug: lakefs-pulls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-pulls-api-openapi.yml
- filename: lakefs-refs-api-openapi.yml
  format: yaml
  label: lakeFS refs API
  slug: lakefs-refs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-refs-api-openapi.yml
- filename: lakefs-repositories-api-openapi.yml
  format: yaml
  label: lakeFS repositories API
  slug: lakefs-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-repositories-api-openapi.yml
- filename: lakefs-staging-api-openapi.yml
  format: yaml
  label: lakeFS staging API
  slug: lakefs-staging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-staging-api-openapi.yml
- filename: lakefs-tags-api-openapi.yml
  format: yaml
  label: lakeFS tags API
  slug: lakefs-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-tags-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lakefs Authentication
name_suffix: Authentication
oauth_flows: []
overview: lakeFS secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: lakeFS
provider_slug: lakefs
scheme_count: 5
schemes:
- name: basic_auth
  scheme: basic
  sources:
  - openapi/lakefs-openapi.yml
  type: http
- bearerFormat: JWT
  name: jwt_token
  scheme: bearer
  sources:
  - openapi/lakefs-openapi.yml
  type: http
- in: cookie
  name: cookie_auth
  parameter: internal_auth_session
  sources:
  - openapi/lakefs-openapi.yml
  type: apiKey
- in: cookie
  name: oidc_auth
  parameter: oidc_auth_session
  sources:
  - openapi/lakefs-openapi.yml
  type: apiKey
- in: cookie
  name: saml_auth
  parameter: saml_auth_session
  sources:
  - openapi/lakefs-openapi.yml
  type: apiKey
slug: lakefs-authentication
source_filename: lakefs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lakefs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/lakefs-openapi.yml\n- name: jwt_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/lakefs-openapi.yml\n- name: cookie_auth\n  type: apiKey\n  in: cookie\n  parameter: internal_auth_session\n  sources:\n  - openapi/lakefs-openapi.yml\n- name: oidc_auth\n  type: apiKey\n  in: cookie\n  parameter: oidc_auth_session\n  sources:\n  - openapi/lakefs-openapi.yml\n- name: saml_auth\n  type: apiKey\n  in: cookie\n  parameter: saml_auth_session\n  sources:\n  - openapi/lakefs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/authentication/lakefs-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Data Version Control
- Data Lake
- Git-like
- Open Source
---
