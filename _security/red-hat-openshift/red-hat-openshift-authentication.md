---
api_key_in: []
api_specs:
- filename: red-hat-openshift-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Container Platform API
  slug: openshift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-api-openapi.yml
- filename: openapi
  format: yaml
  label: Red Hat OpenShift Cluster Manager API
  slug: openshift-cluster-manager-api
  spec_type: OpenAPI
  url: https://api.openshift.com/openapi
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Red Hat Openshift Authentication
name_suffix: Authentication
oauth_flows: []
overview: Red Hat OpenShift secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Red Hat OpenShift
provider_slug: red-hat-openshift
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/red-hat-openshift-api-openapi.yml
  - openapi/red-hat-openshift-cluster-manager-openapi.yml
  type: http
slug: red-hat-openshift-authentication
source_filename: red-hat-openshift-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/red-hat-openshift-api-openapi.yml, openapi/red-hat-openshift-cluster-manager-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/red-hat-openshift-api-openapi.yml\n  - openapi/red-hat-openshift-cluster-manager-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/authentication/red-hat-openshift-authentication.yml
summary_line: http · 1 scheme
tags:
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- PaaS
- Red Hat
---
