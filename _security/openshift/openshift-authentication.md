---
api_key_in: []
api_specs:
- filename: swagger.json
  format: json
  label: OpenShift REST API
  slug: openshift-rest-api
  spec_type: OpenAPI
  url: https://api.openshift.com/api/swagger.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Openshift Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenShift secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenShift
provider_slug: openshift
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth bearer token obtained from the OpenShift OAuth server. Use 'oc whoami -t' to retrieve a token, or configure an OAuth client for programmatic access.
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/openshift-rest-api-openapi.yml
  type: http
slug: openshift-authentication
source_filename: openshift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openshift-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth bearer token obtained from the OpenShift OAuth server. Use 'oc whoami -t'\n    to retrieve a token, or configure an OAuth client for programmatic access.\n  sources:\n  - openapi/openshift-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/authentication/openshift-authentication.yml
summary_line: http · 1 scheme
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
---
