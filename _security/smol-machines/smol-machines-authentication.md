---
api_key_in: []
api_specs:
- filename: smol-machines-apikeys-api-openapi.yml
  format: yaml
  label: Smol Machines apikeys API
  slug: smol-machines-apikeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-apikeys-api-openapi.yml
- filename: smol-machines-apps-api-openapi.yml
  format: yaml
  label: Smol Machines apps API
  slug: smol-machines-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-apps-api-openapi.yml
- filename: smol-machines-billing-api-openapi.yml
  format: yaml
  label: Smol Machines billing API
  slug: smol-machines-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-billing-api-openapi.yml
- filename: smol-machines-containers-api-openapi.yml
  format: yaml
  label: Smol Machines Containers API
  slug: smol-machines-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-containers-api-openapi.yml
- filename: smol-machines-execution-api-openapi.yml
  format: yaml
  label: Smol Machines Execution API
  slug: smol-machines-execution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-execution-api-openapi.yml
- filename: smol-machines-health-api-openapi.yml
  format: yaml
  label: Smol Machines health API
  slug: smol-machines-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-health-api-openapi.yml
- filename: smol-machines-images-api-openapi.yml
  format: yaml
  label: Smol Machines Images API
  slug: smol-machines-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-images-api-openapi.yml
- filename: smol-machines-logs-api-openapi.yml
  format: yaml
  label: Smol Machines Logs API
  slug: smol-machines-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-logs-api-openapi.yml
- filename: smol-machines-machines-api-openapi.yml
  format: yaml
  label: Smol Machines machines API
  slug: smol-machines-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-machines-api-openapi.yml
- filename: smol-machines-microvms-api-openapi.yml
  format: yaml
  label: Smol Machines MicroVMs API
  slug: smol-machines-microvms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-microvms-api-openapi.yml
- filename: smol-machines-nodes-api-openapi.yml
  format: yaml
  label: Smol Machines nodes API
  slug: smol-machines-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-nodes-api-openapi.yml
- filename: smol-machines-operations-api-openapi.yml
  format: yaml
  label: Smol Machines operations API
  slug: smol-machines-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-operations-api-openapi.yml
- filename: smol-machines-plans-api-openapi.yml
  format: yaml
  label: Smol Machines plans API
  slug: smol-machines-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-plans-api-openapi.yml
- filename: smol-machines-pools-api-openapi.yml
  format: yaml
  label: Smol Machines pools API
  slug: smol-machines-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-pools-api-openapi.yml
- filename: smol-machines-sandboxes-api-openapi.yml
  format: yaml
  label: Smol Machines Sandboxes API
  slug: smol-machines-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-sandboxes-api-openapi.yml
- filename: smol-machines-tenants-api-openapi.yml
  format: yaml
  label: Smol Machines tenants API
  slug: smol-machines-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-tenants-api-openapi.yml
- filename: smol-machines-tokens-api-openapi.yml
  format: yaml
  label: Smol Machines tokens API
  slug: smol-machines-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-tokens-api-openapi.yml
- filename: smol-machines-usage-api-openapi.yml
  format: yaml
  label: Smol Machines usage API
  slug: smol-machines-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-usage-api-openapi.yml
- filename: smol-machines-volumes-api-openapi.yml
  format: yaml
  label: Smol Machines volumes API
  slug: smol-machines-volumes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-volumes-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Smol Machines Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: Smol Machines secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: Smol Machines
provider_slug: smol-machines
scheme_count: 3
schemes:
- applies_to: https://api.smolmachines.com (smolfleet cloud REST API — /v1/*)
  description: 'All hosted Cloud API endpoints require an Authorization: Bearer <api_key> header. Keys are created in the console (smolmachines.com/console) or via POST /v1/apikeys, are prefixed smk_, and are exported by convention as SMOLCLOUD_KEY. Managed via /v1/apikeys and /v1/tokens.'
  docs: https://smolmachines.com/docs/cloud-api
  format: Bearer smk_<api_key>
  header: Authorization
  in: header
  name: CloudBearerApiKey
  scheme: bearer
  type: http
- applies_to: smol CLI (`smol auth login`) — registry + smolfleet
  description: The smol CLI authenticates via an OAuth device flow (`smol auth login`); one token covers both the artifact registry and the smolfleet API.
  flow: deviceCode
  in: header
  name: CloudDeviceFlow
  type: oauth2
- applies_to: smolvm local API (`smolvm serve start`, default 127.0.0.1:8080) and the in-process embedded engine used by the SDKs — no auth on the loopback interface; isolation is enforced by the hypervisor boundary, not tokens.
  name: LocalNone
  type: none
slug: smol-machines-authentication
source_filename: smol-machines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://smolmachines.com/docs/cloud-api, https://smolmachines.com/docs/cloud-quickstart, https://github.com/smol-machines/smol/blob/main/docs/cli.md\ndocs: https://smolmachines.com/docs/cloud-api\nsummary:\n  types: [http, oauth2]\n  http_scheme: bearer\n  token_prefix: smk_\n  oauth2_flows: [deviceCode]\n  notes: >-\n    Neither published OpenAPI declares components.securitySchemes, so this\n    profile is captured from the provider's documentation, not derived.\nschemes:\n- name: CloudBearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: \"Bearer smk_<api_key>\"\n  applies_to: https://api.smolmachines.com (smolfleet cloud REST API — /v1/*)\n  docs: https://smolmachines.com/docs/cloud-api\n  description: >-\n    All hosted Cloud API endpoints require an Authorization: Bearer <api_key>\n    header. Keys are created in the console (smolmachines.com/console) or via\n    POST /v1/apikeys,\
  \ are prefixed smk_, and are exported by convention as\n    SMOLCLOUD_KEY. Managed via /v1/apikeys and /v1/tokens.\n- name: CloudDeviceFlow\n  type: oauth2\n  flow: deviceCode\n  in: header\n  applies_to: smol CLI (`smol auth login`) — registry + smolfleet\n  description: >-\n    The smol CLI authenticates via an OAuth device flow (`smol auth login`);\n    one token covers both the artifact registry and the smolfleet API.\n- name: LocalNone\n  type: none\n  applies_to: >-\n    smolvm local API (`smolvm serve start`, default 127.0.0.1:8080) and the\n    in-process embedded engine used by the SDKs — no auth on the loopback\n    interface; isolation is enforced by the hypervisor boundary, not tokens.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/authentication/smol-machines-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- MicroVM
- Sandbox
- Virtualization
- Developer Tools
- Infrastructure
- AI Agents
- Code Execution
- Containers
- Cloud
---
