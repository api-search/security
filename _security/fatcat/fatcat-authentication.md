---
api_key_in:
- header
api_specs:
- filename: fatcat-auth-api-openapi.yml
  format: yaml
  label: Fatcat auth API
  slug: fatcat-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatcat/refs/heads/main/openapi/fatcat-auth-api-openapi.yml
- filename: fatcat-changelog-api-openapi.yml
  format: yaml
  label: Fatcat changelog API
  slug: fatcat-changelog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatcat/refs/heads/main/openapi/fatcat-changelog-api-openapi.yml
- filename: fatcat-containers-api-openapi.yml
  format: yaml
  label: Fatcat containers API
  slug: fatcat-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatcat/refs/heads/main/openapi/fatcat-containers-api-openapi.yml
- filename: fatcat-creators-api-openapi.yml
  format: yaml
  label: Fatcat creators API
  slug: fatcat-creators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatcat/refs/heads/main/openapi/fatcat-creators-api-openapi.yml
- filename: fatcat-editgroups-api-openapi.yml
  format: yaml
  label: Fatcat editgroups API
  slug: fatcat-editgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatcat/refs/heads/main/openapi/fatcat-editgroups-api-openapi.yml
- filename: fatcat-editors-api-openapi.yml
  format: yaml
  label: Fatcat editors API
  slug: fatcat-editors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatcat/refs/heads/main/openapi/fatcat-editors-api-openapi.yml
- filename: fatcat-files-api-openapi.yml
  format: yaml
  label: Fatcat files API
  slug: fatcat-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatcat/refs/heads/main/openapi/fatcat-files-api-openapi.yml
- filename: fatcat-filesets-api-openapi.yml
  format: yaml
  label: Fatcat filesets API
  slug: fatcat-filesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatcat/refs/heads/main/openapi/fatcat-filesets-api-openapi.yml
- filename: fatcat-releases-api-openapi.yml
  format: yaml
  label: Fatcat releases API
  slug: fatcat-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatcat/refs/heads/main/openapi/fatcat-releases-api-openapi.yml
- filename: fatcat-webcaptures-api-openapi.yml
  format: yaml
  label: Fatcat webcaptures API
  slug: fatcat-webcaptures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatcat/refs/heads/main/openapi/fatcat-webcaptures-api-openapi.yml
- filename: fatcat-works-api-openapi.yml
  format: yaml
  label: Fatcat works API
  slug: fatcat-works-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fatcat/refs/heads/main/openapi/fatcat-works-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fatcat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fatcat secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fatcat
provider_slug: fatcat
scheme_count: 1
schemes:
- description: "The only current API authentication mechanism is HTTP bearer\nauthentication using the `Authorization` HTTP header. The header should\nbe formatted as the string \"Bearer\", then a space, then API token (in the\nusual base64 string encoding).\n\nAn example HTTP request would look on the wire like:\n\n    GET /v0/auth/check HTTP/1.1\n    Accept: */*\n    Accept-Encoding: gzip, deflate\n    Authorization: Beare"
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/openapi.yml
  type: apiKey
slug: fatcat-authentication
source_filename: fatcat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    The only current API authentication mechanism is HTTP bearer\n    authentication using the `Authorization` HTTP header. The header should\n    be formatted as the string \"Bearer\", then a space, then API token (in the\n    usual base64 string encoding).\n\n    An example HTTP request would look on the wire like:\n\n        GET /v0/auth/check HTTP/1.1\n        Accept: */*\n        Accept-Encoding: gzip, deflate\n        Authorization: Beare\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fatcat/refs/heads/main/authentication/fatcat-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Scholarly
- Research
- Academic
- Open Access
- Bibliographic
- Publications
- Metadata
- Internet Archive
---
