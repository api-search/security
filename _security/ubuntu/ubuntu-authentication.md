---
api_key_in: []
api_specs:
- filename: ubuntu-launchpad-openapi.yml
  format: yaml
  label: Launchpad API
  slug: launchpad-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-launchpad-openapi.yml
- filename: ubuntu-snap-store-openapi.yml
  format: yaml
  label: Snap Store API
  slug: snap-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-snap-store-openapi.yml
- filename: ubuntu-cve-openapi.yml
  format: yaml
  label: Ubuntu CVE API
  slug: ubuntu-cve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-cve-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ubuntu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ubuntu secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ubuntu
provider_slug: ubuntu
scheme_count: 1
schemes:
- description: OAuth 1.0a authentication with Launchpad credentials
  name: OAuth1
  scheme: oauth
  sources:
  - openapi/ubuntu-launchpad-openapi.yml
  type: http
slug: ubuntu-authentication
source_filename: ubuntu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ubuntu-launchpad-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: OAuth1\n  type: http\n  scheme: oauth\n  description: OAuth 1.0a authentication with Launchpad credentials\n  sources:\n  - openapi/ubuntu-launchpad-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/authentication/ubuntu-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud
- Containers
- Devops
- Enterprise
- Linux
- Security
- Ubuntu
- Package Management
- Open Source
---
