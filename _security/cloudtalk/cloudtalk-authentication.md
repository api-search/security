---
api_key_in: []
api_specs:
- filename: cloudtalk-agents-api-openapi.yml
  format: yaml
  label: CloudTalk Agents API
  slug: cloudtalk-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-agents-api-openapi.yml
- filename: cloudtalk-bulks-api-openapi.yml
  format: yaml
  label: CloudTalk Bulks API
  slug: cloudtalk-bulks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-bulks-api-openapi.yml
- filename: cloudtalk-calls-api-openapi.yml
  format: yaml
  label: CloudTalk Calls API
  slug: cloudtalk-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-calls-api-openapi.yml
- filename: cloudtalk-campaigns-api-openapi.yml
  format: yaml
  label: CloudTalk Campaigns API
  slug: cloudtalk-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-campaigns-api-openapi.yml
- filename: cloudtalk-contacts-api-openapi.yml
  format: yaml
  label: CloudTalk Contacts API
  slug: cloudtalk-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-contacts-api-openapi.yml
- filename: cloudtalk-conversation-intelligence-api-openapi.yml
  format: yaml
  label: CloudTalk Conversation Intelligence API
  slug: cloudtalk-conversation-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-conversation-intelligence-api-openapi.yml
- filename: cloudtalk-cuecard-api-openapi.yml
  format: yaml
  label: CloudTalk CueCard API
  slug: cloudtalk-cuecard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-cuecard-api-openapi.yml
- filename: cloudtalk-groups-api-openapi.yml
  format: yaml
  label: CloudTalk Groups API
  slug: cloudtalk-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-groups-api-openapi.yml
- filename: cloudtalk-numbers-api-openapi.yml
  format: yaml
  label: CloudTalk Numbers API
  slug: cloudtalk-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-numbers-api-openapi.yml
- filename: cloudtalk-other-api-openapi.yml
  format: yaml
  label: CloudTalk Other API
  slug: cloudtalk-other-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-other-api-openapi.yml
- filename: cloudtalk-sms-api-openapi.yml
  format: yaml
  label: CloudTalk Sms API
  slug: cloudtalk-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-sms-api-openapi.yml
- filename: cloudtalk-tags-api-openapi.yml
  format: yaml
  label: CloudTalk Tags API
  slug: cloudtalk-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-tags-api-openapi.yml
- filename: cloudtalk-voiceagent-api-openapi.yml
  format: yaml
  label: CloudTalk VoiceAgent API
  slug: cloudtalk-voiceagent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-voiceagent-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cloudtalk Authentication
name_suffix: Authentication
oauth_flows: []
overview: CloudTalk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CloudTalk
provider_slug: cloudtalk
scheme_count: 1
schemes:
- description: 'HTTPS-only HTTP Basic Authentication. The username is the API Access Key ID and the password is the Access Key Secret, passed as an `Authorization: Basic <base64(id:secret)>` header. The Basic Auth credential pair also determines which project the request executes against. Credentials are created by Administrators in the CloudTalk Dashboard under Account -> Settings -> API keys.'
  example: curl -u ACCESS_KEY_ID:ACCESS_KEY_SECRET https://my.cloudtalk.io/api/calls/index.json
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/cloudtalk-openapi.json
  type: http
slug: cloudtalk-authentication
source_filename: cloudtalk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.cloudtalk.io/\ndocs: https://developers.cloudtalk.io/\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  note: The published OpenAPI (v1.7) declares no components.securitySchemes; the auth model\n    below is captured from the CloudTalk API reference documentation.\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: >-\n    HTTPS-only HTTP Basic Authentication. The username is the API Access Key ID and the\n    password is the Access Key Secret, passed as an `Authorization: Basic <base64(id:secret)>`\n    header. The Basic Auth credential pair also determines which project the request executes\n    against. Credentials are created by Administrators in the CloudTalk Dashboard under\n    Account -> Settings -> API keys.\n  example: \"curl -u ACCESS_KEY_ID:ACCESS_KEY_SECRET https://my.cloudtalk.io/api/calls/index.json\"\n  sources: [openapi/cloudtalk-openapi.json]\n\
  scopes_model: none\nnotes: >-\n  Authentication is account/project-scoped with no token granularity or scopes — a key pair\n  holds full read/write access to the project's data. No OAuth 2.0 or OpenID Connect is offered.\n  There is no documented read-only or scoped credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/authentication/cloudtalk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Communications
- Voice
- VoIP
- Call Center
- Contact Center
- CCaaS
- Telephony
- SMS
- Conversation Intelligence
---
