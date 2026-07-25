---
api_key_in: []
api_specs:
- filename: goharbor-artifacts-api-openapi.yml
  format: yaml
  label: GoHarbor artifacts API
  slug: goharbor-artifacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-artifacts-api-openapi.yml
- filename: goharbor-audit-api-openapi.yml
  format: yaml
  label: GoHarbor audit API
  slug: goharbor-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-audit-api-openapi.yml
- filename: goharbor-health-api-openapi.yml
  format: yaml
  label: GoHarbor health API
  slug: goharbor-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-health-api-openapi.yml
- filename: goharbor-projects-api-openapi.yml
  format: yaml
  label: GoHarbor projects API
  slug: goharbor-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-projects-api-openapi.yml
- filename: goharbor-quotas-api-openapi.yml
  format: yaml
  label: GoHarbor quotas API
  slug: goharbor-quotas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-quotas-api-openapi.yml
- filename: goharbor-registries-api-openapi.yml
  format: yaml
  label: GoHarbor registries API
  slug: goharbor-registries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-registries-api-openapi.yml
- filename: goharbor-replication-api-openapi.yml
  format: yaml
  label: GoHarbor replication API
  slug: goharbor-replication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-replication-api-openapi.yml
- filename: goharbor-repositories-api-openapi.yml
  format: yaml
  label: GoHarbor repositories API
  slug: goharbor-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-repositories-api-openapi.yml
- filename: goharbor-robots-api-openapi.yml
  format: yaml
  label: GoHarbor robots API
  slug: goharbor-robots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-robots-api-openapi.yml
- filename: goharbor-scan-api-openapi.yml
  format: yaml
  label: GoHarbor scan API
  slug: goharbor-scan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-scan-api-openapi.yml
- filename: goharbor-search-api-openapi.yml
  format: yaml
  label: GoHarbor search API
  slug: goharbor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-search-api-openapi.yml
- filename: goharbor-tags-api-openapi.yml
  format: yaml
  label: GoHarbor tags API
  slug: goharbor-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-tags-api-openapi.yml
- filename: goharbor-usergroups-api-openapi.yml
  format: yaml
  label: GoHarbor usergroups API
  slug: goharbor-usergroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-usergroups-api-openapi.yml
- filename: goharbor-webhooks-api-openapi.yml
  format: yaml
  label: GoHarbor webhooks API
  slug: goharbor-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/openapi/goharbor-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Goharbor Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoHarbor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GoHarbor
provider_slug: goharbor
scheme_count: 1
schemes:
- description: Harbor user credentials (HTTP Basic)
  name: basicAuth
  scheme: basic
  sources:
  - openapi/goharbor-openapi.yml
  type: http
slug: goharbor-authentication
source_filename: goharbor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/goharbor-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Harbor user credentials (HTTP Basic)\n  sources:\n  - openapi/goharbor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goharbor/refs/heads/main/authentication/goharbor-authentication.yml
summary_line: http · 1 scheme
tags:
- Container Registry
---
