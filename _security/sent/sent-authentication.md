---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Sent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sent declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Sent
provider_slug: sent
scheme_count: 2
schemes:
- evidence: The Sent API v3 authenticates every request with an API key. Send it in the x-api-key header, or as a Bearer token in the Authorization header.
  header: x-api-key
  location: header
  name: x-api-key
  type: apiKey
- evidence: The Sent API v3 authenticates every request with an API key. Send it in the x-api-key header, or as a Bearer token in the Authorization header.
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
slug: sent-authentication
source_filename: sent-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.sent.dm/reference/api/authentication
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.sent.dm/reference/api/authentication\nsources:\n- https://docs.sent.dm/reference/api/authentication\n- https://docs.sent.dm/reference/api/channels/SentDmServicesEndpointsCustomerAPIv3ChannelsCreateVoiceTokenEndpoint\n- https://docs.sent.dm/reference/api/webhooks/SentDmServicesEndpointsCustomerAPIv3WebhooksRotateWebhookSecretEndpoint\n- https://docs.sent.dm/reference/api/profiles/SentDmServicesEndpointsCustomerAPIv3ProfilesCompleteProfileEndpoint\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: The Sent API v3 authenticates every request with an API key. Send it in the x-api-key header, or as a Bearer token in the Authorization\n    header.\n  location: header\n  header: x-api-key\n- type: http-bearer\n  name: Authorization\n  evidence: The Sent API v3 authenticates every request with an API key. Send it in the x-api-key header, or as a Bearer token in the Authorization\n\
  \    header.\n  location: header\n  header: Authorization\ndocs: https://docs.sent.dm/reference/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/sent/authentication/sent-authentication.yml
summary_line: 2 schemes
tags:
- SMS
- WhatsApp
- RCS
- Messaging API
- Communications
- Developer Platform
- Authentication
- Order Notifications
---
