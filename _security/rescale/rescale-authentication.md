---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Rescale Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rescale secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rescale
provider_slug: rescale
scheme_count: 4
schemes:
- format: Token <api-token>
  in: header
  name: RescaleRestToken
  parameter: Authorization
  type: apiKey
  used_by: Rescale REST API v2 (platform.rescale.com/api/v2/)
- in: header
  name: RescaleMcpApiKey
  parameter: X-Rescale-Api-Key
  type: apiKey
  used_by: Rescale hosted MCP server
- bearer_format: JWT
  name: RescaleHtcBearer
  notes: The HTC API uses JWT bearer tokens obtained from API/refresh tokens; the rescalehtc library auto-renews them and supports multiple workspaces.
  scheme: bearer
  type: http
  used_by: Rescale HTC API (rescalehtc client; rauthenticate CLI manages refresh tokens)
- in: env
  name: RescaleJobEmbeddedKey
  notes: Jobs receive a temporary RESCALE_API_KEY environment variable scoped to the job that expires after the job completes.
  parameter: RESCALE_API_KEY
  type: apiKey
  used_by: In-job post-processing
slug: rescale-authentication
source_filename: rescale-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://rescale.com/documentation/main/rescale-advanced-features/rest-api/\ndocs: https://rescale.com/documentation/main/platform-faqs/api-faq/\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header]\n  notes: >-\n    Rescale uses token-based authentication. API keys are generated from the\n    Rescale platform (Profile > User Profile Settings > API > Add API Key, or\n    Settings > API Key at platform.rescale.com/user/settings/). There is no\n    OAuth2/OIDC surface documented.\nschemes:\n- name: RescaleRestToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Token <api-token>'\n  used_by: Rescale REST API v2 (platform.rescale.com/api/v2/)\n- name: RescaleMcpApiKey\n  type: apiKey\n  in: header\n  parameter: X-Rescale-Api-Key\n  used_by: Rescale hosted MCP server\n- name: RescaleHtcBearer\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  used_by: Rescale HTC API (rescalehtc client; rauthenticate\
  \ CLI manages refresh tokens)\n  notes: >-\n    The HTC API uses JWT bearer tokens obtained from API/refresh tokens; the\n    rescalehtc library auto-renews them and supports multiple workspaces.\n- name: RescaleJobEmbeddedKey\n  type: apiKey\n  in: env\n  parameter: RESCALE_API_KEY\n  used_by: In-job post-processing\n  notes: >-\n    Jobs receive a temporary RESCALE_API_KEY environment variable scoped to the\n    job that expires after the job completes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rescale/refs/heads/main/authentication/rescale-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- High Performance Computing
- Simulation
- Cloud
- Engineering
- CAE
- HPC
- AI Physics
- Jobs
- Compute
---
