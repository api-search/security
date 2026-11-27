---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cuevr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cuevr declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cuevr
provider_slug: cuevr-com
scheme_count: 1
schemes:
- description: Organization access keys created by an owner or administrator in Admin > Organization > Integrations > Access keys. The key starts with cuevr_ and is scoped to selected permissions. It is shown only once at creation.
  name: organization-access-key
  placement: null
  placement_note: The public docs do not state the header or parameter that carries the key, and they do not publish a base URL.
  prefix: cuevr_
  rotation: Renew the key creates a new key with the same permissions, and the old key keeps working for the period shown in the confirmation window. Revoke the key stops it immediately. Keys created by a member who leaves the organization, or who is no longer an administrator, are revoked.
  scoped: true
  type: apiKey
  verification: Documented key verification route ("Test the connection with the key verification route"); its path is not published.
slug: cuevr-com-authentication
source_filename: cuevr-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Cuevr authentication\ngenerated: '2026-11-04'\nmethod: searched\nsource: https://www.cuevr.com/getting-started/integrations\ndocs: https://www.cuevr.com/getting-started/integrations\nschemes:\n- name: organization-access-key\n  type: apiKey\n  description: Organization access keys created by an owner or administrator in Admin > Organization > Integrations > Access keys. The key starts with cuevr_ and is scoped to selected permissions. It is shown only once at creation.\n  prefix: cuevr_\n  scoped: true\n  placement: null\n  placement_note: The public docs do not state the header or parameter that carries the key, and they do not publish a base URL.\n  rotation: Renew the key creates a new key with the same permissions, and the old key keeps working for the period shown in the confirmation window. Revoke the key stops it immediately. Keys created by a member who leaves the organization, or who is no longer an administrator, are revoked.\n  verification: Documented key\
  \ verification route (\"Test the connection with the key verification route\"); its path is not published.\nwebhook_signing:\n  algorithm: HMAC-SHA256\n  header: X-Cuevr-Signature\n  timestamp_header: X-Cuevr-Timestamp\n  previous_signature_header: X-Cuevr-Signature-Previous\n  description: An HMAC-SHA256 signature of the timestamp and the body, computed with the destination's secret. During secret renewal, deliveries are signed with both secrets.\n"
source_yaml_url: https://artifacts.apis.io/cuevr-com/authentication/cuevr-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Sales Proposals
- E-Signature
- RFP
- Sales Enablement
- Artificial Intelligence
- MCP
- Webhook
---
