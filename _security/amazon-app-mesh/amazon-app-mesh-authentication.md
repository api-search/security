---
api_key_in:
- header
api_specs:
- filename: amazon-app-mesh-meshes-api-openapi.yml
  format: yaml
  label: Amazon App Mesh Meshes API
  slug: amazon-app-mesh-meshes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/openapi/amazon-app-mesh-meshes-api-openapi.yml
- filename: amazon-app-mesh-tag-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon App Mesh Tag#resourceArn API
  slug: amazon-app-mesh-tag-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/openapi/amazon-app-mesh-tag-resourcearn-api-openapi.yml
- filename: amazon-app-mesh-tags-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon App Mesh Tags#resourceArn API
  slug: amazon-app-mesh-tags-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/openapi/amazon-app-mesh-tags-resourcearn-api-openapi.yml
- filename: amazon-app-mesh-untag-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon App Mesh Untag#resourceArn API
  slug: amazon-app-mesh-untag-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/openapi/amazon-app-mesh-untag-resourcearn-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon App Mesh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon App Mesh secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon App Mesh
provider_slug: amazon-app-mesh
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-app-mesh-openapi.json
  - openapi/amazon-app-mesh-openapi.yaml
  type: apiKey
slug: amazon-app-mesh-authentication
source_filename: amazon-app-mesh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-app-mesh-openapi.json, openapi/amazon-app-mesh-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-app-mesh-openapi.json\n  - openapi/amazon-app-mesh-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-app-mesh/refs/heads/main/authentication/amazon-app-mesh-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Microservices
- Networking
- Service Mesh
---
