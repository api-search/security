---
api_key_in: []
api_specs:
- filename: vagrant-cloud-api-openapi.yml
  format: yaml
  label: Vagrant Cloud API
  slug: vagrant-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagrant/refs/heads/main/openapi/vagrant-cloud-api-openapi.yml
- filename: vagrant-hcp-vagrant-box-registry-openapi.yml
  format: yaml
  label: HCP Vagrant Box Registry API
  slug: vagrant-hcp-box-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vagrant/refs/heads/main/openapi/vagrant-hcp-vagrant-box-registry-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vagrant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vagrant secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vagrant
provider_slug: vagrant
scheme_count: 1
schemes:
- description: Vagrant Cloud API token passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/vagrant-cloud-api-openapi.yml
  - openapi/vagrant-hcp-vagrant-box-registry-openapi.yml
  type: http
slug: vagrant-authentication
source_filename: vagrant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vagrant-cloud-api-openapi.yml, openapi/vagrant-hcp-vagrant-box-registry-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Vagrant Cloud API token passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/vagrant-cloud-api-openapi.yml\n  - openapi/vagrant-hcp-vagrant-box-registry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vagrant/refs/heads/main/authentication/vagrant-authentication.yml
summary_line: http · 1 scheme
tags:
- DevOps
- Virtualization
- Development Environments
- Boxes
- Cloud
- HashiCorp
- Infrastructure
---
