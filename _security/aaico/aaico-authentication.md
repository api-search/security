---
anonymous_access: false
api_key_in: []
api_specs:
- filename: postman-collection
  format: yaml
  label: Opus Platform API
  slug: opus-platform-api
  spec_type: Postman
  url: https://developer.opus.com/api-reference/v0-jobs/postman-collection
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aaico Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppliedAI (AAICO) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AppliedAI (AAICO)
provider_slug: aaico
scheme_count: 1
schemes:
- applies_to: all endpoints
  description: A single static service key sent on every request. The key carries the acting user's identity, their organization, and the workspaces they can target; each endpoint additionally requires a named permission in the target workspace.
  id: serviceKey
  in: header
  name: x-service-key
  required: true
  scoped: false
  type: apiKey
slug: aaico-authentication
source_filename: aaico-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://developer.opus.com/api-reference/quickstart\ndocs:\n- https://developer.opus.com/api-reference/introduction\n- https://developer.opus.com/api-reference/quickstart\n- https://developer.opus.com/api-reference/v1-case/case-introduction\n- https://developer.opus.com/api-reference/v1-integration/integration-introduction\napi: Opus Platform API\nbase_url: https://operator.opus.com/api/v1\nnote: >-\n  Derived from the published API reference, not from an OpenAPI document — AAICO publishes no\n  machine-readable spec for the Opus platform API (see conformance/). The scheme below was also\n  confirmed live: an unauthenticated GET of https://operator.opus.com/api/v1 returns HTTP 401\n  with {\"statusCode\":401,\"message\":\"API key is required\"}.\nschemes:\n- id: serviceKey\n  type: apiKey\n  in: header\n  name: x-service-key\n  required: true\n  description: >-\n    A single static service key sent on every request. The key\
  \ carries the acting user's identity,\n    their organization, and the workspaces they can target; each endpoint additionally requires a\n    named permission in the target workspace.\n  applies_to: all endpoints\n  scoped: false\noauth2: false\nopenid_connect: false\nmutual_tls: false\nbasic_auth: false\nbearer_token: false\nx-evidence:\n  probe:\n    url: https://operator.opus.com/api/v1\n    method: GET\n    http_status: 401\n    body: '{\"statusCode\":401,\"message\":\"API key is required\",\"timestamp\":\"...\",\"path\":\"/api/v1\"}'\n    fetched: '2026-09-05'\nkey_management:\n  self_service: true\n  console_path: Opus button (top left) -> Channels -> API\n  create: '+ Generate API Key, with a key name and a required expiry'\n  shown_once: true\n  rotation: manual; keys are deleted and regenerated from the API page\n  expiry: required at creation (Key Expiry field)\n  listed_metadata: [name, creation date, expiration date, last used date]\n  revoke: Delete from the API page\n  docs:\
  \ https://developer.opus.com/api-reference/quickstart\npermissions:\n  model: named permissions granted per workspace, plus organization-level grants\n  observed:\n  - name: 'Workflow: Full'\n    level: workspace\n    required_by: [generate workflow, cancel run, get run status, get workflow details]\n  - name: 'Integration: Full'\n    level: organization\n    required_by: [create provider, create integration, add credential]\n    note: >-\n      Explicitly organization-level — a workspace-level grant is not sufficient, because\n      integrations belong to the organization rather than to a workspace.\nfailure_modes:\n- status: 401\n  when: missing, invalid or expired key, or the key's user is no longer a member of the organization\n- status: 403\n  when: the key is valid but the user lacks the required permission in the target workspace/organization\ngaps:\n- No OAuth 2.0 or OpenID Connect surface, so there is no delegated/third-party authorization path.\n- No scope system — permissions\
  \ are console-granted roles, not token scopes, so scopes/ is not applicable.\n- Keys are not prefixed, so a leaked key is not identifiable by shape.\n- No documented programmatic key-management endpoints; keys are created and revoked in the UI only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aaico/refs/heads/main/authentication/aaico-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Workflow Automation
- Agents
- Enterprise
- Document Processing
- Regulated Industries
- Business Process Automation
- Banking
- Insurance
- Healthcare
- Model Context Protocol
---
