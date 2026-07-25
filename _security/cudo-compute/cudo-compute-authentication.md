---
api_key_in: []
api_specs:
- filename: cudo-compute-billing-api-openapi.yml
  format: yaml
  label: CUDO Compute Billing API
  slug: cudo-compute-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-billing-api-openapi.yml
- filename: cudo-compute-data-centers-api-openapi.yml
  format: yaml
  label: CUDO Compute Data Centers API
  slug: cudo-compute-data-centers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-data-centers-api-openapi.yml
- filename: cudo-compute-disks-api-openapi.yml
  format: yaml
  label: CUDO Compute Disks API
  slug: cudo-compute-disks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-disks-api-openapi.yml
- filename: cudo-compute-images-api-openapi.yml
  format: yaml
  label: CUDO Compute Images API
  slug: cudo-compute-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-images-api-openapi.yml
- filename: cudo-compute-machine-types-api-openapi.yml
  format: yaml
  label: CUDO Compute Machine Types API
  slug: cudo-compute-machine-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-machine-types-api-openapi.yml
- filename: cudo-compute-networks-api-openapi.yml
  format: yaml
  label: CUDO Compute Networks API
  slug: cudo-compute-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-networks-api-openapi.yml
- filename: cudo-compute-ssh-keys-api-openapi.yml
  format: yaml
  label: CUDO Compute SSH Keys API
  slug: cudo-compute-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-ssh-keys-api-openapi.yml
- filename: cudo-compute-virtual-machines-api-openapi.yml
  format: yaml
  label: CUDO Compute Virtual Machines API
  slug: cudo-compute-virtual-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-virtual-machines-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cudo Compute Authentication
name_suffix: Authentication
oauth_flows: []
overview: CUDO Compute secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CUDO Compute
provider_slug: cudo-compute
scheme_count: 1
schemes:
- description: 'A CUDO Compute API key passed as a Bearer token in the Authorization header, e.g. `Authorization: Bearer $CUDO_API_KEY`. Create keys in the CUDO Compute dashboard. Missing or invalid keys return 401 UNAUTHENTICATED.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cudo-compute-openapi.yml
  type: http
slug: cudo-compute-authentication
source_filename: cudo-compute-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cudo-compute-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A CUDO Compute API key passed as a Bearer token in the Authorization header,\n    e.g. `Authorization: Bearer $CUDO_API_KEY`. Create keys in the CUDO Compute dashboard. Missing\n    or invalid keys return 401 UNAUTHENTICATED.'\n  sources:\n  - openapi/cudo-compute-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/authentication/cudo-compute-authentication.yml
summary_line: http · 1 scheme
tags:
- GPU
- Cloud Compute
- Infrastructure
- Virtual Machines
- Marketplace
---
