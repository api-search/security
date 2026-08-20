---
api_key_in: []
api_specs:
- filename: openrelay-account-api-openapi.yml
  format: yaml
  label: OpenRelay Account API
  slug: openrelay-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-account-api-openapi.yml
- filename: openrelay-api-keys-api-openapi.yml
  format: yaml
  label: OpenRelay API Keys API
  slug: openrelay-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-api-keys-api-openapi.yml
- filename: openrelay-batches-api-openapi.yml
  format: yaml
  label: OpenRelay Batches API
  slug: openrelay-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-batches-api-openapi.yml
- filename: openrelay-billing-api-openapi.yml
  format: yaml
  label: OpenRelay Billing API
  slug: openrelay-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-billing-api-openapi.yml
- filename: openrelay-catalog-api-openapi.yml
  format: yaml
  label: OpenRelay Catalog API
  slug: openrelay-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-catalog-api-openapi.yml
- filename: openrelay-clusters-api-openapi.yml
  format: yaml
  label: OpenRelay Clusters API
  slug: openrelay-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-clusters-api-openapi.yml
- filename: openrelay-files-api-openapi.yml
  format: yaml
  label: OpenRelay Files API
  slug: openrelay-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-files-api-openapi.yml
- filename: openrelay-internal-api-openapi.yml
  format: yaml
  label: OpenRelay Internal API
  slug: openrelay-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-internal-api-openapi.yml
- filename: openrelay-organizations-api-openapi.yml
  format: yaml
  label: OpenRelay Organizations API
  slug: openrelay-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-organizations-api-openapi.yml
- filename: openrelay-provider-api-openapi.yml
  format: yaml
  label: OpenRelay Provider API
  slug: openrelay-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-provider-api-openapi.yml
- filename: openrelay-registry-credentials-api-openapi.yml
  format: yaml
  label: OpenRelay Registry Credentials API
  slug: openrelay-registry-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-registry-credentials-api-openapi.yml
- filename: openrelay-runners-api-openapi.yml
  format: yaml
  label: OpenRelay Runners API
  slug: openrelay-runners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-runners-api-openapi.yml
- filename: openrelay-snapshots-api-openapi.yml
  format: yaml
  label: OpenRelay Snapshots API
  slug: openrelay-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-snapshots-api-openapi.yml
- filename: openrelay-ssh-keys-api-openapi.yml
  format: yaml
  label: OpenRelay SSH Keys API
  slug: openrelay-ssh-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-ssh-keys-api-openapi.yml
- filename: openrelay-transfers-api-openapi.yml
  format: yaml
  label: OpenRelay Transfers API
  slug: openrelay-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-transfers-api-openapi.yml
- filename: openrelay-usage-api-openapi.yml
  format: yaml
  label: OpenRelay Usage API
  slug: openrelay-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-usage-api-openapi.yml
- filename: openrelay-vms-api-openapi.yml
  format: yaml
  label: OpenRelay VMs API
  slug: openrelay-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-vms-api-openapi.yml
- filename: openrelay-webhooks-api-openapi.yml
  format: yaml
  label: OpenRelay Webhooks API
  slug: openrelay-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/openapi/openrelay-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Openrelay Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenRelay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: OpenRelay
provider_slug: openrelay
scheme_count: 1
schemes:
- alt_header: x-api-key (Inference API only)
  description: 'OpenRelay API key. Send it as `Authorization: Bearer vl_…`.'
  docs: https://docs.openrelay.inc/docs/authentication
  key_prefix: vl_
  name: apiKey
  scheme: bearer
  sources:
  - openapi/openrelay-openapi.json
  - https://docs.openrelay.inc/docs/authentication
  type: http
slug: openrelay-authentication
source_filename: openrelay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/openrelay-openapi.json\ndocs: https://docs.openrelay.inc/docs/authentication\nsummary:\n  types:\n  - http\n  notes: >-\n    Single auth model. Every control-plane request is authenticated with an\n    OpenRelay API key (prefix `vl_`) sent as an HTTP Bearer token. Keys are\n    org-scoped and created in the dashboard under Settings -> API Keys; the\n    plaintext is shown once. The Inference API additionally accepts the same\n    key via an `x-api-key` header for OpenAI-SDK compatibility. No OAuth2 /\n    OIDC flows are offered.\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  key_prefix: vl_\n  description: 'OpenRelay API key. Send it as `Authorization: Bearer vl_…`.'\n  alt_header: x-api-key (Inference API only)\n  docs: https://docs.openrelay.inc/docs/authentication\n  sources:\n  - openapi/openrelay-openapi.json\n  - https://docs.openrelay.inc/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openrelay/refs/heads/main/authentication/openrelay-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- GPU
- Inference
- Artificial Intelligence
- Machine-Learning
- Cloud Compute
- Infrastructure
- OpenAI-Compatible
- GPU Cloud
- LLM
---
