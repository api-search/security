---
api_key_in: []
api_specs:
- filename: simplivity-backups-api-openapi.yml
  format: yaml
  label: SimpliVity backups API
  slug: simplivity-backups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-backups-api-openapi.yml
- filename: simplivity-cluster-groups-api-openapi.yml
  format: yaml
  label: SimpliVity cluster_groups API
  slug: simplivity-cluster-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-cluster-groups-api-openapi.yml
- filename: simplivity-datastores-api-openapi.yml
  format: yaml
  label: SimpliVity datastores API
  slug: simplivity-datastores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-datastores-api-openapi.yml
- filename: simplivity-external-stores-api-openapi.yml
  format: yaml
  label: SimpliVity external_stores API
  slug: simplivity-external-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-external-stores-api-openapi.yml
- filename: simplivity-hosts-api-openapi.yml
  format: yaml
  label: SimpliVity hosts API
  slug: simplivity-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-hosts-api-openapi.yml
- filename: simplivity-omnistack-clusters-api-openapi.yml
  format: yaml
  label: SimpliVity omnistack_clusters API
  slug: simplivity-omnistack-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-omnistack-clusters-api-openapi.yml
- filename: simplivity-policies-api-openapi.yml
  format: yaml
  label: SimpliVity policies API
  slug: simplivity-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-policies-api-openapi.yml
- filename: simplivity-security-api-openapi.yml
  format: yaml
  label: SimpliVity security API
  slug: simplivity-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-security-api-openapi.yml
- filename: simplivity-tasks-api-openapi.yml
  format: yaml
  label: SimpliVity tasks API
  slug: simplivity-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-tasks-api-openapi.yml
- filename: simplivity-virtual-machines-api-openapi.yml
  format: yaml
  label: SimpliVity virtual_machines API
  slug: simplivity-virtual-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/openapi/simplivity-virtual-machines-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Simplivity Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: SimpliVity secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: SimpliVity
provider_slug: simplivity
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 2
    tokenUrl: /oauth/token
  name: OAuth2
  sources:
  - openapi/simplivity-omnistack-openapi-original.json
  type: oauth2
slug: simplivity-authentication
source_filename: simplivity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/simplivity-omnistack-openapi-original.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: /oauth/token\n    scopes: 2\n  sources:\n  - openapi/simplivity-omnistack-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplivity/refs/heads/main/authentication/simplivity-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Big Data
- Hyperconverged Infrastructure
- Virtualization
- Backup
- Disaster Recovery
- Data-Center
- Storage
- Cloud Infrastructure
- HPE
---
