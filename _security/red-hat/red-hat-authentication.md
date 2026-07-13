---
api_key_in: []
api_specs:
- filename: openapi
  format: yaml
  label: Red Hat OpenShift API
  slug: red-hat-openshift-api
  spec_type: OpenAPI
  url: https://api.openshift.com/api/clusters_mgmt/v1/openapi
- filename: openapi
  format: yaml
  label: Red Hat OpenShift Cluster Manager API
  slug: red-hat-openshift-cluster-manager-api
  spec_type: OpenAPI
  url: https://api.openshift.com/api/clusters_mgmt/v1/openapi
- filename: red-hat-ansible-automation-platform-openapi.yml
  format: yaml
  label: Red Hat Ansible Automation Platform API
  slug: red-hat-ansible-automation-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/openapi/red-hat-ansible-automation-platform-openapi.yml
- filename: discovery
  format: yaml
  label: Red Hat Quay API
  slug: red-hat-quay-api
  spec_type: OpenAPI
  url: https://quay.io/api/v1/discovery
- filename: red-hat-insights-openapi.yml
  format: yaml
  label: Red Hat Insights API
  slug: red-hat-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/openapi/red-hat-insights-openapi.yml
- filename: red-hat-satellite-openapi.yml
  format: yaml
  label: Red Hat Satellite API
  slug: red-hat-satellite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/openapi/red-hat-satellite-openapi.yml
- filename: red-hat-keycloak-admin-openapi.yml
  format: yaml
  label: Red Hat Build of Keycloak Admin REST API
  slug: red-hat-build-of-keycloak-admin-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/openapi/red-hat-keycloak-admin-openapi.yml
- filename: red-hat-kafka-bridge-asyncapi.yml
  format: yaml
  label: Red Hat Streams for Apache Kafka Bridge API
  slug: red-hat-streams-for-apache-kafka-bridge-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/asyncapi/red-hat-kafka-bridge-asyncapi.yml
- filename: red-hat-notifications-webhooks-asyncapi.yml
  format: yaml
  label: Red Hat Notifications API
  slug: red-hat-notifications-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/asyncapi/red-hat-notifications-webhooks-asyncapi.yml
- filename: openapi
  format: yaml
  label: Red Hat Assisted Installer API
  slug: red-hat-assisted-installer-api
  spec_type: OpenAPI
  url: https://api.openshift.com/api/assisted-install/v2/openapi
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Red Hat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Red Hat secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Red Hat
provider_slug: red-hat
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth 2.0 Bearer token for authenticating API requests to the automation controller.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/red-hat-ansible-automation-platform-openapi.yml
  - openapi/red-hat-insights-openapi.yml
  - openapi/red-hat-keycloak-admin-openapi.yml
  - openapi/red-hat-openshift-cluster-manager-openapi.yml
  - openapi/red-hat-quay-openapi.yml
  type: http
- description: HTTP Basic Authentication using a valid Satellite username and password. Alternatively, a personal access token can be used.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/red-hat-satellite-openapi.yml
  type: http
slug: red-hat-authentication
source_filename: red-hat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/red-hat-ansible-automation-platform-openapi.yml, openapi/red-hat-insights-openapi.yml,\n  openapi/red-hat-keycloak-admin-openapi.yml, openapi/red-hat-openshift-cluster-manager-openapi.yml,\n  openapi/red-hat-quay-openapi.yml, openapi/red-hat-satellite-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 Bearer token for authenticating API requests to the automation controller.\n  sources:\n  - openapi/red-hat-ansible-automation-platform-openapi.yml\n  - openapi/red-hat-insights-openapi.yml\n  - openapi/red-hat-keycloak-admin-openapi.yml\n  - openapi/red-hat-openshift-cluster-manager-openapi.yml\n  - openapi/red-hat-quay-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using a valid Satellite username and password. Alternatively,\n    a personal access token can be used.\n\
  \  sources:\n  - openapi/red-hat-satellite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/authentication/red-hat-authentication.yml
summary_line: http · 2 schemes
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
---
