---
anonymous_access: false
api_key_in: []
api_specs:
- filename: temp-md-openapi.yml
  format: yaml
  label: temp.md Public API
  slug: tempmd-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temp-md/refs/heads/main/openapi/temp-md-openapi.yml
- filename: temp-md-platform-openapi.yml
  format: yaml
  label: temp.md Embedded Preview Platform API
  slug: tempmd-embedded-preview-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temp-md/refs/heads/main/openapi/temp-md-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 7
method: searched
name: Temp Md Authentication
name_suffix: Authentication
oauth_flows: []
overview: temp.md secures its APIs with http across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: temp.md
provider_slug: temp-md
scheme_count: 7
schemes:
- accepted_on:
  - updateTemp
  - revokeTemp
  - createPublishSession (tempId update)
  - getTempStatus
  - restoreTemp
  - snapshotTemp
  - updateTempCapabilitySettings
  bearerFormat: tempmd scoped capability
  name: tempCapability
  obtained_from: response of POST /temps (updateToken, claimToken) or POST /publish-sessions/{id}/finalize
  rotation: Claiming a Temp into an account ROTATES the update token; the old one stops working (docs#privacy, skill.md). rotateUpdateToken invalidates every prior token and returns one replacement exactly once.
  scheme: bearer
  sources:
  - openapi/temp-md-openapi.yml
  type: http
  what_it_is: The per-Temp updateToken returned by createTemp / finalizePublishSession (or the claimToken for status/restore). Prefix observed in docs examples "tempmd_...".
- accepted_on:
  - getPublishSession
  - uploadPublishSessionFile
  - finalizePublishSession
  bearerFormat: tempmd_upload session capability
  name: publishSessionToken
  scheme: bearer
  sources:
  - openapi/temp-md-openapi.yml
  type: http
  what_it_is: One-hour upload capability (PublishSession.uploadToken) minted by createPublishSession.
- accepted_on:
  - revokeTemp
  - createPublishSession
  - getTempStatus
  - restoreTemp
  - snapshotTemp
  - updateTempCapabilitySettings
  - listApiKeys
  - createApiKey
  - revokeApiKey
  - rotateUpdateToken
  - MCP connection header (list_temps
  - recover_update_token
  - account-owned publish)
  - A2A GetTask/ListTasks
  bearerFormat: JWT or tempmd_key API key
  key_management: GET/POST /me/api-keys, DELETE /me/api-keys/{keyId}; CLI `tempmd login`, `tempmd keys`, `tempmd keys revoke <id>`
  name: accountBearer
  scheme: bearer
  sources:
  - openapi/temp-md-openapi.yml
  - https://temp.md/.well-known/agent.json
  type: http
  what_it_is: Account session token from POST /auth/login (LoginResult.token) or a named API key created with POST /me/api-keys (prefix tempmd_key_, secret shown once, stored hashed, max 20 active keys).
- accepted_on:
  - createOrganization
  - getOrganization
  - createApplication
  - getApplication
  - updateApplication
  - listApplicationKeys
  - createApplicationKey
  - revokeApplicationKey
  - webhook endpoint + domain binding operations
  description: A Temp.md dashboard session or personal account API key.
  name: dashboardBearer
  scheme: bearer
  sources:
  - openapi/temp-md-platform-openapi.yml
  type: http
- accepted_on:
  - listPlatformPreviews
  - getPlatformPreview
  - revokePlatformPreview
  - createPublishGrant
  - revokePublishGrant
  - createPlatformPublishSession
  - listReviewRequests
  - createReviewRequest
  - getPlatformUsage
  bearerFormat: tempmd_app_<id>_<secret>
  description: Server-only Application key with explicit scopes. Returned once; must never reach a browser or Electron renderer.
  name: applicationBearer
  scheme: bearer
  sources:
  - openapi/temp-md-platform-openapi.yml
  - https://temp.md/llms.txt
  type: http
- accepted_on:
  - createPlatformPublishSession
  bearerFormat: tempmd_grant_<id>_<secret>
  description: Short-lived, one-session delegated publishing authority (backend mints a 5-15 minute grant; requests carrying an Origin header MUST use a grant, not an Application key).
  name: publishGrantBearer
  scheme: bearer
  sources:
  - openapi/temp-md-platform-openapi.yml
  - https://temp.md/llms.txt
  type: http
- accepted_on:
  - getReviewRequest
  - createReviewDecision
  bearerFormat: tempmd_view_<id>_<secret>
  description: Short-lived viewer capability bound to one frozen review request.
  name: reviewBearer
  scheme: bearer
  sources:
  - openapi/temp-md-platform-openapi.yml
  type: http
slug: temp-md-authentication
source_filename: temp-md-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/temp-md-openapi.yml, openapi/temp-md-platform-openapi.yml, https://temp.md/docs, https://temp.md/.well-known/agent.json, live probes 2026-09-19\ndocs: https://temp.md/docs#publish\nsummary:\n  types: [http]\n  schemes_count: 7\n  anonymous_publish: true\n  oauth2: false\n  note: >-\n    Everything is HTTP Bearer, and the interesting part is WHICH token: temp.md is capability-based. An anonymous\n    POST /temps returns a scoped updateToken (and claimToken) that is the only credential needed to update,\n    inspect, snapshot, restore or revoke that one Temp. Accounts are optional; an account session JWT or a named\n    API key (prefix tempmd_key_) owns Temps, recovers lost update tokens and manages keys. The partner platform\n    adds server-only Application keys (tempmd_app_<id>_<secret>, one-time reveal, explicit scopes), short-lived\n    delegated publish grants (tempmd_grant_...) for browsers, and review-viewer capabilities\
  \ (tempmd_view_...).\n    The derive-authentication.py baseline collapsed these to one scheme because all share type http/bearer;\n    this file lists each with its bearerFormat and where it is accepted.\nanonymous_operations:\n  note: No credential at all (security absent or an empty {} alternative in the spec)\n  operations: [createTemp, createPublishSession (anonymous alternative), listTempComments, appendTempComments, signup, login, reportAbuse, getHealth, getA2AAgentCard, sendA2AJsonRpc (publish), MCP tools/list + publish_temp]\nschemes:\n- name: tempCapability\n  type: http\n  scheme: bearer\n  bearerFormat: tempmd scoped capability\n  what_it_is: The per-Temp updateToken returned by createTemp / finalizePublishSession (or the claimToken for status/restore). Prefix observed in docs examples \"tempmd_...\".\n  obtained_from: response of POST /temps (updateToken, claimToken) or POST /publish-sessions/{id}/finalize\n  accepted_on: [updateTemp, revokeTemp, createPublishSession (tempId\
  \ update), getTempStatus, restoreTemp, snapshotTemp, updateTempCapabilitySettings]\n  rotation: Claiming a Temp into an account ROTATES the update token; the old one stops working (docs#privacy, skill.md). rotateUpdateToken invalidates every prior token and returns one replacement exactly once.\n  sources: [openapi/temp-md-openapi.yml]\n- name: publishSessionToken\n  type: http\n  scheme: bearer\n  bearerFormat: tempmd_upload session capability\n  what_it_is: One-hour upload capability (PublishSession.uploadToken) minted by createPublishSession.\n  accepted_on: [getPublishSession, uploadPublishSessionFile, finalizePublishSession]\n  sources: [openapi/temp-md-openapi.yml]\n- name: accountBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT or tempmd_key API key\n  what_it_is: Account session token from POST /auth/login (LoginResult.token) or a named API key created with POST /me/api-keys (prefix tempmd_key_, secret shown once, stored hashed, max 20 active keys).\n  accepted_on: [revokeTemp,\
  \ createPublishSession, getTempStatus, restoreTemp, snapshotTemp, updateTempCapabilitySettings, listApiKeys, createApiKey, revokeApiKey, rotateUpdateToken, MCP connection header (list_temps, recover_update_token, account-owned publish), A2A GetTask/ListTasks]\n  key_management: GET/POST /me/api-keys, DELETE /me/api-keys/{keyId}; CLI `tempmd login`, `tempmd keys`, `tempmd keys revoke <id>`\n  sources: [openapi/temp-md-openapi.yml, https://temp.md/.well-known/agent.json]\n- name: dashboardBearer\n  type: http\n  scheme: bearer\n  description: A Temp.md dashboard session or personal account API key.\n  accepted_on: [createOrganization, getOrganization, createApplication, getApplication, updateApplication, listApplicationKeys, createApplicationKey, revokeApplicationKey, webhook endpoint + domain binding operations]\n  sources: [openapi/temp-md-platform-openapi.yml]\n- name: applicationBearer\n  type: http\n  scheme: bearer\n  bearerFormat: tempmd_app_<id>_<secret>\n  description: Server-only\
  \ Application key with explicit scopes. Returned once; must never reach a browser or Electron renderer.\n  accepted_on: [listPlatformPreviews, getPlatformPreview, revokePlatformPreview, createPublishGrant, revokePublishGrant, createPlatformPublishSession, listReviewRequests, createReviewRequest, getPlatformUsage]\n  sources: [openapi/temp-md-platform-openapi.yml, https://temp.md/llms.txt]\n- name: publishGrantBearer\n  type: http\n  scheme: bearer\n  bearerFormat: tempmd_grant_<id>_<secret>\n  description: Short-lived, one-session delegated publishing authority (backend mints a 5-15 minute grant; requests carrying an Origin header MUST use a grant, not an Application key).\n  accepted_on: [createPlatformPublishSession]\n  sources: [openapi/temp-md-platform-openapi.yml, https://temp.md/llms.txt]\n- name: reviewBearer\n  type: http\n  scheme: bearer\n  bearerFormat: tempmd_view_<id>_<secret>\n  description: Short-lived viewer capability bound to one frozen review request.\n  accepted_on:\
  \ [getReviewRequest, createReviewDecision]\n  sources: [openapi/temp-md-platform-openapi.yml]\nheaders:\n  authorization: 'Authorization: Bearer <token>'\n  client_identity: 'X-Tempmd-Client: product/version (optional, sanitized attribution only; pattern ^[A-Za-z0-9][A-Za-z0-9._+/@-]{0,79}$; never user data or capabilities)'\ncors:\n  note: Capability-backed publish-session, status, update and revoke routes allow credential-free cross-origin requests; account, claim, settings, restore, snapshot and dashboard routes keep a restricted-origin policy. Do not send cookies. (docs#browser-integrations)\nsignup:\n  self_serve: true\n  operations: [signup, login]\n  dashboard: https://temp.md/dashboard\n  note: Not required to publish.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temp-md/refs/heads/main/authentication/temp-md-authentication.yml
summary_line: http · 7 schemes
tags:
- Web Publishing
- Static Hosting
- AI Agents
- MCP
- A2A
- Developer Tools
- Preview Infrastructure
- File Sharing
- Agent-Native
- Company
---
