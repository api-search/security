---
api_key_in: []
api_specs:
- filename: openshift-routes-api-openapi.yml
  format: yaml
  label: OpenShift Routes API
  slug: openshift-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/openapi/openshift-routes-api-openapi.yml
- filename: openshift-buildconfigs-api-openapi.yml
  format: yaml
  label: OpenShift BuildConfigs API
  slug: openshift-buildconfigs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/openapi/openshift-buildconfigs-api-openapi.yml
- filename: openshift-builds-api-openapi.yml
  format: yaml
  label: OpenShift Builds API
  slug: openshift-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/openapi/openshift-builds-api-openapi.yml
- filename: openshift-deploymentconfigs-api-openapi.yml
  format: yaml
  label: OpenShift DeploymentConfigs API
  slug: openshift-deploymentconfigs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/openapi/openshift-deploymentconfigs-api-openapi.yml
- filename: openshift-projectrequests-api-openapi.yml
  format: yaml
  label: OpenShift ProjectRequests API
  slug: openshift-projectrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/openapi/openshift-projectrequests-api-openapi.yml
- filename: openshift-projects-api-openapi.yml
  format: yaml
  label: OpenShift Projects API
  slug: openshift-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/openapi/openshift-projects-api-openapi.yml
- filename: openshift-routes-api-openapi.yml
  format: yaml
  label: OpenShift Routes API
  slug: openshift-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/openapi/openshift-routes-api-openapi.yml
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
- Cloud-Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
---
