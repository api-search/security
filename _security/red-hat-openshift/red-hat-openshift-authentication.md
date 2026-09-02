---
api_key_in: []
api_specs:
- filename: red-hat-openshift-add-ons-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Add-ons API
  slug: red-hat-openshift-add-ons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-add-ons-api-openapi.yml
- filename: red-hat-openshift-builds-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Builds API
  slug: red-hat-openshift-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-builds-api-openapi.yml
- filename: red-hat-openshift-clusters-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Clusters API
  slug: red-hat-openshift-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-clusters-api-openapi.yml
- filename: red-hat-openshift-deployment-configs-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Deployment Configs API
  slug: red-hat-openshift-deployment-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-deployment-configs-api-openapi.yml
- filename: red-hat-openshift-identity-providers-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Identity Providers API
  slug: red-hat-openshift-identity-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-identity-providers-api-openapi.yml
- filename: red-hat-openshift-image-streams-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Image Streams API
  slug: red-hat-openshift-image-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-image-streams-api-openapi.yml
- filename: red-hat-openshift-machine-pools-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Machine Pools API
  slug: red-hat-openshift-machine-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-machine-pools-api-openapi.yml
- filename: red-hat-openshift-projects-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Projects API
  slug: red-hat-openshift-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-projects-api-openapi.yml
- filename: red-hat-openshift-routes-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Routes API
  slug: red-hat-openshift-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-routes-api-openapi.yml
- filename: red-hat-openshift-security-context-constraints-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Security Context Constraints API
  slug: red-hat-openshift-security-context-constraints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-security-context-constraints-api-openapi.yml
- filename: red-hat-openshift-versions-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Versions API
  slug: red-hat-openshift-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-versions-api-openapi.yml
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
- Platform-as-a-Service
- Red Hat
---
