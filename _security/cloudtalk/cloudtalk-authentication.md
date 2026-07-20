---
api_key_in: []
api_specs:
- filename: cloudtalk-openapi.json
  format: json
  label: CloudTalk API
  slug: cloudtalk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudtalk/refs/heads/main/openapi/cloudtalk-openapi.json
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
