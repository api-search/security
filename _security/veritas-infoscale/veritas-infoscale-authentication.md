---
api_key_in: []
api_specs:
- filename: veritas-infoscale-alerts-api-openapi.yml
  format: yaml
  label: Veritas InfoScale Alerts API
  slug: veritas-infoscale-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/openapi/veritas-infoscale-alerts-api-openapi.yml
- filename: veritas-infoscale-clusters-api-openapi.yml
  format: yaml
  label: Veritas InfoScale Clusters API
  slug: veritas-infoscale-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/openapi/veritas-infoscale-clusters-api-openapi.yml
- filename: veritas-infoscale-disk-groups-api-openapi.yml
  format: yaml
  label: Veritas InfoScale Disk Groups API
  slug: veritas-infoscale-disk-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/openapi/veritas-infoscale-disk-groups-api-openapi.yml
- filename: veritas-infoscale-disks-api-openapi.yml
  format: yaml
  label: Veritas InfoScale Disks API
  slug: veritas-infoscale-disks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/openapi/veritas-infoscale-disks-api-openapi.yml
- filename: veritas-infoscale-fencing-api-openapi.yml
  format: yaml
  label: Veritas InfoScale Fencing API
  slug: veritas-infoscale-fencing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/openapi/veritas-infoscale-fencing-api-openapi.yml
- filename: veritas-infoscale-jobs-api-openapi.yml
  format: yaml
  label: Veritas InfoScale Jobs API
  slug: veritas-infoscale-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/openapi/veritas-infoscale-jobs-api-openapi.yml
- filename: veritas-infoscale-resources-api-openapi.yml
  format: yaml
  label: Veritas InfoScale Resources API
  slug: veritas-infoscale-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/openapi/veritas-infoscale-resources-api-openapi.yml
- filename: veritas-infoscale-service-groups-api-openapi.yml
  format: yaml
  label: Veritas InfoScale Service Groups API
  slug: veritas-infoscale-service-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/openapi/veritas-infoscale-service-groups-api-openapi.yml
- filename: veritas-infoscale-systems-api-openapi.yml
  format: yaml
  label: Veritas InfoScale Systems API
  slug: veritas-infoscale-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/openapi/veritas-infoscale-systems-api-openapi.yml
- filename: veritas-infoscale-volumes-api-openapi.yml
  format: yaml
  label: Veritas InfoScale Volumes API
  slug: veritas-infoscale-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/openapi/veritas-infoscale-volumes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Veritas Infoscale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Veritas InfoScale secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Veritas InfoScale
provider_slug: veritas-infoscale
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token authentication for InfoScale REST API
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/veritas-infoscale-rest-api.yaml
  type: http
slug: veritas-infoscale-authentication
source_filename: veritas-infoscale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/veritas-infoscale-rest-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token authentication for InfoScale REST API\n  sources:\n  - openapi/veritas-infoscale-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veritas-infoscale/refs/heads/main/authentication/veritas-infoscale-authentication.yml
summary_line: http · 1 scheme
tags:
- Clustering
- Data Management
- Disaster Recovery
- High Availability
- Storage Management
- Virtualization
---
