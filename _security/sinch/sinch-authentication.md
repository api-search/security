---
api_key_in: []
api_specs:
- filename: sinch-sms-openapi.yml
  format: yaml
  label: Sinch SMS API
  slug: sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch/refs/heads/main/openapi/sinch-sms-openapi.yml
- filename: sinch-conversation-openapi.yml
  format: yaml
  label: Sinch Conversation API
  slug: conversation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch/refs/heads/main/openapi/sinch-conversation-openapi.yml
- filename: sinch-voice-openapi.yml
  format: yaml
  label: Sinch Voice API
  slug: voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch/refs/heads/main/openapi/sinch-voice-openapi.yml
- filename: sinch-verification-openapi.yml
  format: yaml
  label: Sinch Verification API
  slug: verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch/refs/heads/main/openapi/sinch-verification-openapi.yml
- filename: sinch-numbers-openapi.yml
  format: yaml
  label: Sinch Numbers API
  slug: numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch/refs/heads/main/openapi/sinch-numbers-openapi.yml
- filename: sinch-fax-openapi.yml
  format: yaml
  label: Sinch Fax API
  slug: fax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch/refs/heads/main/openapi/sinch-fax-openapi.yml
- filename: sinch-elastic-sip-trunking-openapi.yml
  format: yaml
  label: Sinch Elastic SIP Trunking API
  slug: elastic-sip-trunking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch/refs/heads/main/openapi/sinch-elastic-sip-trunking-openapi.yml
- filename: sinch-brands-openapi.yml
  format: yaml
  label: Sinch Brands API
  slug: brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch/refs/heads/main/openapi/sinch-brands-openapi.yml
- filename: sinch-provisioning-openapi.yml
  format: yaml
  label: Sinch Provisioning API
  slug: provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch/refs/heads/main/openapi/sinch-provisioning-openapi.yml
- filename: sinch-registration-openapi.yml
  format: yaml
  label: Sinch Registration API
  slug: registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sinch/refs/heads/main/openapi/sinch-registration-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sinch Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Sinch secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Sinch
provider_slug: sinch
scheme_count: 3
schemes:
- description: Bearer token authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sinch-brands-openapi.yml
  - openapi/sinch-sms-openapi.yml
  type: http
- description: OAuth 2.0 client credentials flow using project key ID and secret.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.sinch.com/oauth2/token
  name: oAuth2
  sources:
  - openapi/sinch-conversation-openapi.yml
  - openapi/sinch-elastic-sip-trunking-openapi.yml
  - openapi/sinch-fax-openapi.yml
  - openapi/sinch-numbers-openapi.yml
  - openapi/sinch-provisioning-openapi.yml
  - openapi/sinch-registration-openapi.yml
  type: oauth2
- description: Key ID as username and key secret as password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/sinch-conversation-openapi.yml
  - openapi/sinch-elastic-sip-trunking-openapi.yml
  - openapi/sinch-fax-openapi.yml
  - openapi/sinch-numbers-openapi.yml
  - openapi/sinch-provisioning-openapi.yml
  - openapi/sinch-verification-openapi.yml
  - openapi/sinch-voice-openapi.yml
  type: http
slug: sinch-authentication
source_filename: sinch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sinch-brands-openapi.yml, openapi/sinch-conversation-openapi.yml, openapi/sinch-elastic-sip-trunking-openapi.yml,\n  openapi/sinch-fax-openapi.yml, openapi/sinch-numbers-openapi.yml, openapi/sinch-provisioning-openapi.yml,\n  openapi/sinch-registration-openapi.yml, openapi/sinch-sms-openapi.yml, openapi/sinch-verification-openapi.yml,\n  openapi/sinch-voice-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication.\n  sources:\n  - openapi/sinch-brands-openapi.yml\n  - openapi/sinch-sms-openapi.yml\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.sinch.com/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 client credentials flow using project key ID and secret.\n  sources:\n  - openapi/sinch-conversation-openapi.yml\n  - openapi/sinch-elastic-sip-trunking-openapi.yml\n\
  \  - openapi/sinch-fax-openapi.yml\n  - openapi/sinch-numbers-openapi.yml\n  - openapi/sinch-provisioning-openapi.yml\n  - openapi/sinch-registration-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Key ID as username and key secret as password.\n  sources:\n  - openapi/sinch-conversation-openapi.yml\n  - openapi/sinch-elastic-sip-trunking-openapi.yml\n  - openapi/sinch-fax-openapi.yml\n  - openapi/sinch-numbers-openapi.yml\n  - openapi/sinch-provisioning-openapi.yml\n  - openapi/sinch-verification-openapi.yml\n  - openapi/sinch-voice-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sinch/refs/heads/main/authentication/sinch-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Communications
- Messaging
- SMS
- Voice
- Verification
- CPaaS
---
