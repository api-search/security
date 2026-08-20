---
api_key_in:
- header
api_specs:
- filename: openstack-domains-api-openapi.yml
  format: yaml
  label: OpenStack Domains API
  slug: openstack-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-domains-api-openapi.yml
- filename: openstack-endpoints-api-openapi.yml
  format: yaml
  label: OpenStack Endpoints API
  slug: openstack-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-endpoints-api-openapi.yml
- filename: openstack-flavors-api-openapi.yml
  format: yaml
  label: OpenStack Flavors API
  slug: openstack-flavors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-flavors-api-openapi.yml
- filename: openstack-groups-api-openapi.yml
  format: yaml
  label: OpenStack Groups API
  slug: openstack-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-groups-api-openapi.yml
- filename: openstack-images-api-openapi.yml
  format: yaml
  label: OpenStack Images API
  slug: openstack-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-images-api-openapi.yml
- filename: openstack-keypairs-api-openapi.yml
  format: yaml
  label: OpenStack Keypairs API
  slug: openstack-keypairs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-keypairs-api-openapi.yml
- filename: openstack-projects-api-openapi.yml
  format: yaml
  label: OpenStack Projects API
  slug: openstack-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-projects-api-openapi.yml
- filename: openstack-roles-api-openapi.yml
  format: yaml
  label: OpenStack Roles API
  slug: openstack-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-roles-api-openapi.yml
- filename: openstack-server-actions-api-openapi.yml
  format: yaml
  label: OpenStack Server Actions API
  slug: openstack-server-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-server-actions-api-openapi.yml
- filename: openstack-servers-api-openapi.yml
  format: yaml
  label: OpenStack Servers API
  slug: openstack-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-servers-api-openapi.yml
- filename: openstack-services-api-openapi.yml
  format: yaml
  label: OpenStack Services API
  slug: openstack-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-services-api-openapi.yml
- filename: openstack-tokens-api-openapi.yml
  format: yaml
  label: OpenStack Tokens API
  slug: openstack-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-tokens-api-openapi.yml
- filename: openstack-users-api-openapi.yml
  format: yaml
  label: OpenStack Users API
  slug: openstack-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-users-api-openapi.yml
- filename: openstack-versions-api-openapi.yml
  format: yaml
  label: OpenStack Versions API
  slug: openstack-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-versions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Openstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenStack secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenStack
provider_slug: openstack
scheme_count: 1
schemes:
- in: header
  name: TokenAuth
  parameter: X-Auth-Token
  sources:
  - openapi/openstack-keystone-openapi.yml
  - openapi/openstack-nova-openapi.yml
  type: apiKey
slug: openstack-authentication
source_filename: openstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openstack-keystone-openapi.yml, openapi/openstack-nova-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  sources:\n  - openapi/openstack-keystone-openapi.yml\n  - openapi/openstack-nova-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/authentication/openstack-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Platform
- Infrastructure-as-a-Service
- Open-Source
- Virtualization
- Linux Foundation
---
