---
api_key_in: []
api_specs:
- filename: spruce-health-contact-fields-api-openapi.yml
  format: yaml
  label: Spruce Health Contact Fields API
  slug: spruce-health-contact-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-contact-fields-api-openapi.yml
- filename: spruce-health-contact-tags-api-openapi.yml
  format: yaml
  label: Spruce Health Contact Tags API
  slug: spruce-health-contact-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-contact-tags-api-openapi.yml
- filename: spruce-health-contacts-api-openapi.yml
  format: yaml
  label: Spruce Health Contacts API
  slug: spruce-health-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-contacts-api-openapi.yml
- filename: spruce-health-conversation-item-api-openapi.yml
  format: yaml
  label: Spruce Health Conversation Item API
  slug: spruce-health-conversation-item-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-conversation-item-api-openapi.yml
- filename: spruce-health-conversation-tags-api-openapi.yml
  format: yaml
  label: Spruce Health Conversation Tags API
  slug: spruce-health-conversation-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-conversation-tags-api-openapi.yml
- filename: spruce-health-conversations-api-openapi.yml
  format: yaml
  label: Spruce Health Conversations API
  slug: spruce-health-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-conversations-api-openapi.yml
- filename: spruce-health-internal-endpoints-api-openapi.yml
  format: yaml
  label: Spruce Health Internal Endpoints API
  slug: spruce-health-internal-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-internal-endpoints-api-openapi.yml
- filename: spruce-health-media-api-openapi.yml
  format: yaml
  label: Spruce Health Media API
  slug: spruce-health-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-media-api-openapi.yml
- filename: spruce-health-organization-api-openapi.yml
  format: yaml
  label: Spruce Health Organization API
  slug: spruce-health-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-organization-api-openapi.yml
- filename: spruce-health-phone-lines-api-openapi.yml
  format: yaml
  label: Spruce Health Phone Lines API
  slug: spruce-health-phone-lines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-phone-lines-api-openapi.yml
- filename: spruce-health-saved-messages-api-openapi.yml
  format: yaml
  label: Spruce Health Saved Messages API
  slug: spruce-health-saved-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-saved-messages-api-openapi.yml
- filename: spruce-health-scheduled-messages-api-openapi.yml
  format: yaml
  label: Spruce Health Scheduled Messages API
  slug: spruce-health-scheduled-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-scheduled-messages-api-openapi.yml
- filename: spruce-health-teams-api-openapi.yml
  format: yaml
  label: Spruce Health Teams API
  slug: spruce-health-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-teams-api-openapi.yml
- filename: spruce-health-transcription-api-openapi.yml
  format: yaml
  label: Spruce Health Transcription API
  slug: spruce-health-transcription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-transcription-api-openapi.yml
- filename: spruce-health-webhooks-api-openapi.yml
  format: yaml
  label: Spruce Health Webhooks API
  slug: spruce-health-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/openapi/spruce-health-webhooks-api-openapi.yml
auth_types:
- http
description: 'The Spruce Health API has exactly one credential: a long-lived organization Bearer token. There is no OAuth, no OIDC, no mTLS, no per-user credential and no scope system - a token carries the full permissions of the organization it belongs to. The interesting part of Spruce''s auth posture is not the scheme but the gate in front of it: a token cannot be created at all until Spruce Support has enabled API access for the organization.'
kind: authentication
layout: security
method: searched
name: Spruce Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spruce Health secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spruce Health
provider_slug: spruce-health
scheme_count: 1
schemes:
- applied: globally
  applied_note: Declared at the document root as security[0], so it applies to all 47 operations; no operation opts out and there is no anonymous surface.
  declared_in_spec: true
  description: API token provided by Spruce, passed in an Authorization header with the value "Bearer <token>".
  format: Bearer <your-token>
  header: Authorization
  in: header
  name: spruceAPIToken
  scheme: bearer
  sources:
  - openapi/_original/spruce-health-openapi.json
  - https://developer.sprucehealth.com/docs/overview.md
  type: http
slug: spruce-health-authentication
source_filename: spruce-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: https://developer.sprucehealth.com/docs/overview.md\ndocs: https://developer.sprucehealth.com/docs/overview\nprovider: Spruce Health\nproviderId: spruce-health\ndescription: >-\n  The Spruce Health API has exactly one credential: a long-lived organization Bearer\n  token. There is no OAuth, no OIDC, no mTLS, no per-user credential and no scope\n  system - a token carries the full permissions of the organization it belongs to. The\n  interesting part of Spruce's auth posture is not the scheme but the gate in front of\n  it: a token cannot be created at all until Spruce Support has enabled API access for\n  the organization.\n\nsummary:\n  types:\n  - http\n  schemes_count: 1\n  oauth2: false\n  scopes: false\n  mtls: false\n  self_serve: false\n\nschemes:\n- name: spruceAPIToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <your-token>'\n  description: >-\n    API token provided by\
  \ Spruce, passed in an Authorization header with the value\n    \"Bearer <token>\".\n  declared_in_spec: true\n  applied: globally\n  applied_note: >-\n    Declared at the document root as security[0], so it applies to all 47 operations;\n    no operation opts out and there is no anonymous surface.\n  sources:\n  - openapi/_original/spruce-health-openapi.json\n  - https://developer.sprucehealth.com/docs/overview.md\n\ncredential:\n  subject: organization\n  subject_note: >-\n    The token identifies an organization, not a user. Every call is made as the practice.\n    There is no delegated or per-teammate authorization, so an integration cannot be\n    constrained to one clinician's contacts or act on a specific member's behalf; the\n    author of a posted message is chosen in the request body, not by the credential.\n  lifetime: long-lived\n  rotation: manual\n  rotation_note: >-\n    Administrators generate and manage credentials from the API Access section of\n    Settings. No expiry,\
  \ refresh, or automatic rotation is documented.\n  scopes: none\n  scopes_note: >-\n    No scope, permission or role system exists for API tokens. A token is all-or-nothing\n    across contacts, conversations, messages, media, phone lines, organization members\n    and webhook registration - including the ability to read patient PHI and send\n    outbound messages from the practice's phone and fax numbers.\n\nprovisioning:\n  self_serve: false\n  steps:\n  - step: 1\n    action: Be on the Communicator plan\n    note: API access is a Communicator ($49/user/month) feature; Basic ($24) does not include it.\n  - step: 2\n    action: Request API access from Spruce Support\n    url: https://sprucehealth.com/spruce-api\n    note: >-\n      Access must be enabled for the organization before any token can be generated.\n      This is a human gate, not a form that returns a key.\n  - step: 3\n    action: An administrator generates a token in Settings > API Access\n    note: Only administrators can\
  \ create or manage credentials.\n  fee: none\n  fee_note: There is no separate API access fee beyond the Communicator plan.\n\nfailure_modes:\n- condition: missing, incorrect, or disabled token\n  status: 403\n  documented_in_spec: false\n  note: >-\n    Documented in the API Overview but NOT declared on any operation in the OpenAPI - 403\n    appears on exactly one operation (DeleteConversationItem) and there means a\n    permission failure, not an auth failure. A client generated from the spec alone will\n    have no handler for an authentication failure.\n- condition: 401\n  status: not-used\n  note: Spruce does not return 401. Authentication failure is signalled with 403.\n\nrelated_surfaces:\n- surface: MCP\n  url: https://developer.sprucehealth.com/mcp\n  auth: gated\n  note: >-\n    Returns JSON-RPC error -32001 \"Authorization required\" with no WWW-Authenticate\n    header and no RFC 9728 metadata, so an MCP client cannot discover how to\n    authenticate. The credential is expected\
  \ to be the same organization token.\n  see: mcp/spruce-health-mcp.yml\n- surface: Webhooks\n  auth: hmac-signature\n  note: >-\n    Inbound verification runs the other way - Spruce signs each event with a per-endpoint\n    secret issued once at registration, base64 in X-Spruce-Signature, HMAC-SHA256.\n  see: asyncapi/spruce-health-webhooks.yml\n\nstandards:\n  oauth2: false\n  oidc: false\n  rfc9728: false\n  well_known_metadata: false\n  well_known_note: >-\n    No openid-configuration, oauth-authorization-server or oauth-protected-resource\n    document is served on any Spruce host; all return 404.\n  see: well-known/spruce-health-well-known.yml\n\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spruce-health/refs/heads/main/authentication/spruce-health-authentication.yml
summary_line: http · 1 scheme
tags:
- Healthcare
- HIPAA
- Communications
- Secure Messaging
- Telehealth
- Patient Engagement
- Contacts
- Conversations
- Messaging
- SMS
- Voice
- VoIP
- Fax
- Video
- Webhook
- Scheduling
- Transcription
- EHR Integration
- Compliance
---
