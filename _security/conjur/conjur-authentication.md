---
api_key_in:
- header
api_specs:
- filename: openapi.yml
  format: yaml
  label: Conjur / CyberArk Secrets Manager API
  slug: conjur-cyberark-secrets-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conjur/refs/heads/main/openapi/openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Conjur Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conjur secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Conjur
provider_slug: conjur
scheme_count: 3
schemes:
- description: 'Basic authentication with Conjur username and password (users only)

    or API key (hosts and users).'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/openapi.yml
  type: http
- description: Conjur access token in `Token token=<base64_encoded_token>` format.
  in: header
  name: conjurAuth
  parameter: Authorization
  sources:
  - openapi/openapi.yml
  type: apiKey
- description: 'Conjur Kubernetes authenticator mutual TLS authentication.

    To authenticate using this method, you must provide a trusted client

    certificate'
  name: conjurKubernetesMutualTls
  scheme: mutual
  sources:
  - openapi/openapi.yml
  type: http
slug: conjur-authentication
source_filename: conjur-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    Basic authentication with Conjur username and password (users only)\n    or API key (hosts and users).\n  sources:\n  - openapi/openapi.yml\n- name: conjurAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Conjur access token in `Token token=<base64_encoded_token>` format.\n  sources:\n  - openapi/openapi.yml\n- name: conjurKubernetesMutualTls\n  type: http\n  scheme: mutual\n  description: |-\n    Conjur Kubernetes authenticator mutual TLS authentication.\n    To authenticate using this method, you must provide a trusted client\n    certificate\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conjur/refs/heads/main/authentication/conjur-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Cybersecurity
- Secrets Management
- Identity and Access Management
- DevSecOps
- Kubernetes
- Machine Identity
- Open Source
---
