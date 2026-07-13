---
api_key_in: []
api_specs:
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel Voice Call API
  slug: exotel-voice-call-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel Call Details API
  slug: exotel-call-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel SMS API
  slug: exotel-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel Numbers API
  slug: exotel-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-openapi.yml
  format: yaml
  label: Exotel Campaigns API
  slug: exotel-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/openapi/exotel-openapi.yml
- filename: exotel-asyncapi.yml
  format: yaml
  label: Exotel AgentStream Voice Streaming API
  slug: exotel-agentstream-voice-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/asyncapi/exotel-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: documented
name: Exotel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exotel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Exotel
provider_slug: exotel
scheme_count: 1
schemes:
- description: 'HTTP Basic authentication (RFC 7617). The API Key is the username and the API Token is the password; both, with the Account SID, come from the Exotel Dashboard -> Settings -> API Settings. Credentials may be passed as an `Authorization: Basic base64(<api_key>:<api_token>)` header (recommended for production) or embedded directly in the request URL as `https://<api_key>:<api_token>@<subdomain>/v1/Accounts/<account_sid>/...`. Region subdomains: api.exotel.com (Singapore, default) or api.in.exotel.com (Mumbai/India). The Account SID also appears in every endpoint path.'
  name: basicAuth
  scheme: basic
  sources:
  - https://developer.exotel.com/docs/references/authentication
  - https://developer.exotel.com/api/make-a-call-api
  type: http
slug: exotel-authentication
source_filename: exotel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://developer.exotel.com/docs/references/authentication\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTP Basic authentication (RFC 7617). The API Key is the username and the\n    API Token is the password; both, with the Account SID, come from the\n    Exotel Dashboard -> Settings -> API Settings. Credentials may be passed as\n    an `Authorization: Basic base64(<api_key>:<api_token>)` header (recommended\n    for production) or embedded directly in the request URL as\n    `https://<api_key>:<api_token>@<subdomain>/v1/Accounts/<account_sid>/...`.\n    Region subdomains: api.exotel.com (Singapore, default) or api.in.exotel.com\n    (Mumbai/India). The Account SID also appears in every endpoint path.\n  sources:\n  - https://developer.exotel.com/docs/references/authentication\n  - https://developer.exotel.com/api/make-a-call-api\nnotes: >-\n  The AgentStream\
  \ WebSocket (wss://) surface does not use this API Basic auth:\n  Exotel connects outbound to a developer-hosted endpoint, and any auth is\n  whatever you enforce on your own wss:// endpoint (e.g. a token in the applet\n  URL surfaced back as custom_parameters).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exotel/refs/heads/main/authentication/exotel-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Telephony
- Voice
- SMS
- India
- CPaaS
- Call Center
- IVR
- Numbers
- Communications
- Customer Engagement
---
