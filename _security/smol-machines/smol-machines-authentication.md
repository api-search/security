---
api_key_in: []
api_specs:
- filename: smol-machines-smolfleet-openapi.json
  format: json
  label: Smol Machines Cloud API (smolfleet)
  slug: smol-machines-cloud-api-smolfleet
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smol-machines/refs/heads/main/openapi/smol-machines-smolfleet-openapi.json
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
