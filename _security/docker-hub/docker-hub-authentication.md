---
api_key_in: []
api_specs:
- filename: docker-hub-access-tokens-api-openapi.yml
  format: yaml
  label: Docker Hub access-tokens API
  slug: docker-hub-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-access-tokens-api-openapi.yml
- filename: docker-hub-audit-logs-api-openapi.yml
  format: yaml
  label: Docker Hub audit-logs API
  slug: docker-hub-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-audit-logs-api-openapi.yml
- filename: docker-hub-authentication-api-api-openapi.yml
  format: yaml
  label: Docker Hub authentication-api API
  slug: docker-hub-authentication-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-authentication-api-api-openapi.yml
- filename: docker-hub-groups-api-openapi.yml
  format: yaml
  label: Docker Hub groups API
  slug: docker-hub-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-groups-api-openapi.yml
- filename: docker-hub-invites-api-openapi.yml
  format: yaml
  label: Docker Hub invites API
  slug: docker-hub-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-invites-api-openapi.yml
- filename: docker-hub-org-access-tokens-api-openapi.yml
  format: yaml
  label: Docker Hub org-access-tokens API
  slug: docker-hub-org-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-org-access-tokens-api-openapi.yml
- filename: docker-hub-org-settings-api-openapi.yml
  format: yaml
  label: Docker Hub org-settings API
  slug: docker-hub-org-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-org-settings-api-openapi.yml
- filename: docker-hub-orgs-api-openapi.yml
  format: yaml
  label: Docker Hub orgs API
  slug: docker-hub-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-orgs-api-openapi.yml
- filename: docker-hub-repositories-api-openapi.yml
  format: yaml
  label: Docker Hub repositories API
  slug: docker-hub-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-repositories-api-openapi.yml
- filename: docker-hub-scim-api-openapi.yml
  format: yaml
  label: Docker Hub scim API
  slug: docker-hub-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/openapi/docker-hub-scim-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Docker Hub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Docker Hub secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Docker Hub
provider_slug: docker-hub
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/docker-hub-openapi.yml
  type: http
slug: docker-hub-authentication
source_filename: docker-hub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/docker-hub-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/docker-hub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docker-hub/refs/heads/main/authentication/docker-hub-authentication.yml
summary_line: http · 1 scheme
tags:
- Containers
- DevOps
- Docker
- Registry
---
