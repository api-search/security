---
api_key_in: []
api_specs:
- filename: knative-apis-api-openapi.yml
  format: yaml
  label: Knative Apis API
  slug: knative-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-apis-api-openapi.yml
- filename: knative-brokers-api-openapi.yml
  format: yaml
  label: Knative Brokers API
  slug: knative-brokers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-brokers-api-openapi.yml
- filename: knative-channels-api-openapi.yml
  format: yaml
  label: Knative Channels API
  slug: knative-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-channels-api-openapi.yml
- filename: knative-configurations-api-openapi.yml
  format: yaml
  label: Knative Configurations API
  slug: knative-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-configurations-api-openapi.yml
- filename: knative-domainmappings-api-openapi.yml
  format: yaml
  label: Knative DomainMappings API
  slug: knative-domainmappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-domainmappings-api-openapi.yml
- filename: knative-eventsources-api-openapi.yml
  format: yaml
  label: Knative EventSources API
  slug: knative-eventsources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-eventsources-api-openapi.yml
- filename: knative-eventtypes-api-openapi.yml
  format: yaml
  label: Knative EventTypes API
  slug: knative-eventtypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-eventtypes-api-openapi.yml
- filename: knative-revisions-api-openapi.yml
  format: yaml
  label: Knative Revisions API
  slug: knative-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-revisions-api-openapi.yml
- filename: knative-routes-api-openapi.yml
  format: yaml
  label: Knative Routes API
  slug: knative-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-routes-api-openapi.yml
- filename: knative-subscriptions-api-openapi.yml
  format: yaml
  label: Knative Subscriptions API
  slug: knative-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-subscriptions-api-openapi.yml
- filename: knative-triggers-api-openapi.yml
  format: yaml
  label: Knative Triggers API
  slug: knative-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/openapi/knative-triggers-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Knative Authentication
name_suffix: Authentication
oauth_flows: []
overview: Knative secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Knative
provider_slug: knative
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Kubernetes service account token or user bearer token. RBAC policies control access to Knative Eventing resources.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/knative-eventing-api-openapi.yml
  - openapi/knative-serving-api-openapi.yml
  type: http
slug: knative-authentication
source_filename: knative-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/knative-eventing-api-openapi.yml, openapi/knative-serving-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Kubernetes service account token or user bearer token. RBAC policies control\n    access to Knative Eventing resources.\n  sources:\n  - openapi/knative-eventing-api-openapi.yml\n  - openapi/knative-serving-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knative/refs/heads/main/authentication/knative-authentication.yml
summary_line: http · 1 scheme
tags:
- Auto-Scaling
- Cloud Native
- Event-Driven
- Graduated
- Kubernetes
- Serverless
---
