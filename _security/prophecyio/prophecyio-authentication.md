---
api_key_in: []
api_specs:
- filename: prophecyio-connections-openapi.json
  format: json
  label: Prophecy API
  slug: prophecy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prophecyio/refs/heads/main/openapi/prophecyio-connections-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Prophecyio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prophecy.io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prophecy.io
provider_slug: prophecyio
scheme_count: 1
schemes:
- bearerFormat: PAT
  header: Authorization
  location: header
  name: personalAccessToken
  scheme: bearer
  sources:
  - https://docs.prophecy.ai/api-reference/introduction
  type: http
slug: prophecyio-authentication
source_filename: prophecyio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.prophecy.ai/api-reference/introduction\ndocs: https://docs.prophecy.ai/api-reference/introduction\nsummary:\n  types: [http]\n  scheme: bearer\n  token_kind: personal-access-token\n  notes: >-\n    The Prophecy REST API authenticates with a per-user Personal Access Token\n    (PAT) sent as a bearer token in the request headers. Tokens are generated in\n    the Prophecy UI under Settings > Access Tokens (name + expiration). API\n    permissions are scoped to the token owner's user permissions. The OpenAPI\n    documents published by Prophecy do not declare a securityScheme, so this\n    profile is sourced from the API reference docs rather than derived.\nschemes:\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: PAT\n  location: header\n  header: Authorization\n  sources:\n  - https://docs.prophecy.ai/api-reference/introduction\nidentity:\n  providers: [SAML, LDAP, Microsoft Entra ID,\
  \ Google SSO]\n  mfa: true\n  scim: optional\n  rbac: true\n  docs: https://docs.prophecy.ai/administration/management/authentication/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prophecyio/refs/heads/main/authentication/prophecyio-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Engineering
- Data Pipelines
- ETL
- Apache Spark
- Databricks
- Snowflake
- Low-Code
- Analytics
- AI
- Data Transformation
---
