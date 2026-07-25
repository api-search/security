---
api_key_in: []
api_specs:
- filename: osisoft-pi-assetservers-api-openapi.yml
  format: yaml
  label: osisoft-pi AssetServers API
  slug: osisoft-pi-assetservers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/openapi/osisoft-pi-assetservers-api-openapi.yml
- filename: osisoft-pi-attributes-api-openapi.yml
  format: yaml
  label: osisoft-pi Attributes API
  slug: osisoft-pi-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/openapi/osisoft-pi-attributes-api-openapi.yml
- filename: osisoft-pi-batchrequests-api-openapi.yml
  format: yaml
  label: osisoft-pi BatchRequests API
  slug: osisoft-pi-batchrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/openapi/osisoft-pi-batchrequests-api-openapi.yml
- filename: osisoft-pi-dataservers-api-openapi.yml
  format: yaml
  label: osisoft-pi DataServers API
  slug: osisoft-pi-dataservers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/openapi/osisoft-pi-dataservers-api-openapi.yml
- filename: osisoft-pi-elements-api-openapi.yml
  format: yaml
  label: osisoft-pi Elements API
  slug: osisoft-pi-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/openapi/osisoft-pi-elements-api-openapi.yml
- filename: osisoft-pi-eventframes-api-openapi.yml
  format: yaml
  label: osisoft-pi EventFrames API
  slug: osisoft-pi-eventframes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/openapi/osisoft-pi-eventframes-api-openapi.yml
- filename: osisoft-pi-pipoints-api-openapi.yml
  format: yaml
  label: osisoft-pi PIPoints API
  slug: osisoft-pi-pipoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/openapi/osisoft-pi-pipoints-api-openapi.yml
- filename: osisoft-pi-streams-api-openapi.yml
  format: yaml
  label: osisoft-pi Streams API
  slug: osisoft-pi-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/openapi/osisoft-pi-streams-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Osisoft Pi Authentication
name_suffix: Authentication
oauth_flows: []
overview: osisoft-pi secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: osisoft-pi
provider_slug: osisoft-pi
scheme_count: 2
schemes:
- description: HTTP Basic Authentication
  name: basicAuth
  scheme: basic
  sources:
  - openapi/osisoft-pi-web-api-openapi.yml
  type: http
- description: Kerberos/Windows Integrated Authentication
  name: kerberos
  scheme: negotiate
  sources:
  - openapi/osisoft-pi-web-api-openapi.yml
  type: http
slug: osisoft-pi-authentication
source_filename: osisoft-pi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/osisoft-pi-web-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication\n  sources:\n  - openapi/osisoft-pi-web-api-openapi.yml\n- name: kerberos\n  type: http\n  scheme: negotiate\n  description: Kerberos/Windows Integrated Authentication\n  sources:\n  - openapi/osisoft-pi-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/authentication/osisoft-pi-authentication.yml
summary_line: http · 2 schemes
tags: []
---
