---
api_key_in: []
api_specs:
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Virtual Machines API
  slug: virtual-machines
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Machine Types API
  slug: machine-types
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Data Centers API
  slug: data-centers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Disks & Storage API
  slug: disks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Networks API
  slug: networks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Images API
  slug: images
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute SSH Keys API
  slug: ssh-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
- filename: cudo-compute-openapi.yml
  format: yaml
  label: CUDO Compute Billing API
  slug: billing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cudo-compute/refs/heads/main/openapi/cudo-compute-openapi.yml
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
