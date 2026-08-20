---
api_key_in: []
api_specs:
- filename: nutanix-alerts-api-openapi.yml
  format: yaml
  label: Nutanix Alerts API
  slug: nutanix-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-alerts-api-openapi.yml
- filename: nutanix-categories-api-openapi.yml
  format: yaml
  label: Nutanix Categories API
  slug: nutanix-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-categories-api-openapi.yml
- filename: nutanix-clusters-api-openapi.yml
  format: yaml
  label: Nutanix Clusters API
  slug: nutanix-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-clusters-api-openapi.yml
- filename: nutanix-hosts-api-openapi.yml
  format: yaml
  label: Nutanix Hosts API
  slug: nutanix-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-hosts-api-openapi.yml
- filename: nutanix-images-api-openapi.yml
  format: yaml
  label: Nutanix Images API
  slug: nutanix-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-images-api-openapi.yml
- filename: nutanix-network-security-rules-api-openapi.yml
  format: yaml
  label: Nutanix Network Security Rules API
  slug: nutanix-network-security-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-network-security-rules-api-openapi.yml
- filename: nutanix-projects-api-openapi.yml
  format: yaml
  label: Nutanix Projects API
  slug: nutanix-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-projects-api-openapi.yml
- filename: nutanix-protection-domains-api-openapi.yml
  format: yaml
  label: Nutanix Protection Domains API
  slug: nutanix-protection-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-protection-domains-api-openapi.yml
- filename: nutanix-snapshots-api-openapi.yml
  format: yaml
  label: Nutanix Snapshots API
  slug: nutanix-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-snapshots-api-openapi.yml
- filename: nutanix-storage-containers-api-openapi.yml
  format: yaml
  label: Nutanix Storage Containers API
  slug: nutanix-storage-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-storage-containers-api-openapi.yml
- filename: nutanix-storage-pools-api-openapi.yml
  format: yaml
  label: Nutanix Storage Pools API
  slug: nutanix-storage-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-storage-pools-api-openapi.yml
- filename: nutanix-subnets-api-openapi.yml
  format: yaml
  label: Nutanix Subnets API
  slug: nutanix-subnets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-subnets-api-openapi.yml
- filename: nutanix-virtual-disks-api-openapi.yml
  format: yaml
  label: Nutanix Virtual Disks API
  slug: nutanix-virtual-disks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-virtual-disks-api-openapi.yml
- filename: nutanix-vms-api-openapi.yml
  format: yaml
  label: Nutanix VMs API
  slug: nutanix-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-vms-api-openapi.yml
- filename: nutanix-webhooks-api-openapi.yml
  format: yaml
  label: Nutanix Webhooks API
  slug: nutanix-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/openapi/nutanix-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nutanix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nutanix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nutanix
provider_slug: nutanix
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using Prism Central username and password credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/nutanix-prism-central-v3-openapi.yml
  - openapi/nutanix-prism-element-v2-openapi.yml
  type: http
slug: nutanix-authentication
source_filename: nutanix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nutanix-prism-central-v3-openapi.yml, openapi/nutanix-prism-element-v2-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Prism Central username and password credentials.\n  sources:\n  - openapi/nutanix-prism-central-v3-openapi.yml\n  - openapi/nutanix-prism-element-v2-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nutanix/refs/heads/main/authentication/nutanix-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Management
- Hyper-Converged
- Infrastructure
- Virtualization
- Kubernetes
- Database
---
