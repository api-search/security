---
api_key_in: []
api_specs:
- filename: ubuntu-bugs-api-openapi.yml
  format: yaml
  label: Ubuntu Bugs API
  slug: ubuntu-bugs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-bugs-api-openapi.yml
- filename: ubuntu-categories-api-openapi.yml
  format: yaml
  label: Ubuntu Categories API
  slug: ubuntu-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-categories-api-openapi.yml
- filename: ubuntu-cves-api-openapi.yml
  format: yaml
  label: Ubuntu CVEs API
  slug: ubuntu-cves-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-cves-api-openapi.yml
- filename: ubuntu-distributions-api-openapi.yml
  format: yaml
  label: Ubuntu Distributions API
  slug: ubuntu-distributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-distributions-api-openapi.yml
- filename: ubuntu-info-api-openapi.yml
  format: yaml
  label: Ubuntu Info API
  slug: ubuntu-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-info-api-openapi.yml
- filename: ubuntu-metrics-api-openapi.yml
  format: yaml
  label: Ubuntu Metrics API
  slug: ubuntu-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-metrics-api-openapi.yml
- filename: ubuntu-notices-api-openapi.yml
  format: yaml
  label: Ubuntu Notices API
  slug: ubuntu-notices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-notices-api-openapi.yml
- filename: ubuntu-packages-api-openapi.yml
  format: yaml
  label: Ubuntu Packages API
  slug: ubuntu-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-packages-api-openapi.yml
- filename: ubuntu-people-api-openapi.yml
  format: yaml
  label: Ubuntu People API
  slug: ubuntu-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-people-api-openapi.yml
- filename: ubuntu-projects-api-openapi.yml
  format: yaml
  label: Ubuntu Projects API
  slug: ubuntu-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-projects-api-openapi.yml
- filename: ubuntu-refresh-api-openapi.yml
  format: yaml
  label: Ubuntu Refresh API
  slug: ubuntu-refresh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-refresh-api-openapi.yml
- filename: ubuntu-search-api-openapi.yml
  format: yaml
  label: Ubuntu Search API
  slug: ubuntu-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ubuntu/refs/heads/main/openapi/ubuntu-search-api-openapi.yml
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
- DevOps
- Enterprise
- Linux
- Security
- Ubuntu
- Package Management
- Open-Source
---
