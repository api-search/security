---
api_key_in:
- header
api_specs:
- filename: openstack-keystone-openapi.yml
  format: yaml
  label: OpenStack Identity (Keystone) API
  slug: keystone
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-keystone-openapi.yml
- filename: openstack-nova-openapi.yml
  format: yaml
  label: OpenStack Compute (Nova) API
  slug: nova
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstack/refs/heads/main/openapi/openstack-nova-openapi.yml
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
- Infrastructure as a Service
- Open Source
- Virtualization
- Linux Foundation
---
