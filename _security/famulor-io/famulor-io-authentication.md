---
anonymous_access: false
api_key_in: []
api_specs:
- filename: famulor-io-account-api-openapi.yml
  format: yaml
  label: Famulor Account API
  slug: famulor-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-account-api-openapi.yml
- filename: famulor-io-ai-chatbot-api-openapi.yml
  format: yaml
  label: Famulor AI Chatbot API
  slug: famulor-io-ai-chatbot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-ai-chatbot-api-openapi.yml
- filename: famulor-io-ai-replies-api-openapi.yml
  format: yaml
  label: Famulor AI Replies API
  slug: famulor-io-ai-replies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-ai-replies-api-openapi.yml
- filename: famulor-io-assistants-api-openapi.yml
  format: yaml
  label: Famulor Assistants API
  slug: famulor-io-assistants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-assistants-api-openapi.yml
- filename: famulor-io-automations-api-openapi.yml
  format: yaml
  label: Famulor Automations API
  slug: famulor-io-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-automations-api-openapi.yml
- filename: famulor-io-calls-api-openapi.yml
  format: yaml
  label: Famulor Calls API
  slug: famulor-io-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-calls-api-openapi.yml
- filename: famulor-io-campaigns-api-openapi.yml
  format: yaml
  label: Famulor Campaigns API
  slug: famulor-io-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-campaigns-api-openapi.yml
- filename: famulor-io-conversations-api-openapi.yml
  format: yaml
  label: Famulor Conversations API
  slug: famulor-io-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-conversations-api-openapi.yml
- filename: famulor-io-folders-api-openapi.yml
  format: yaml
  label: Famulor Folders API
  slug: famulor-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-folders-api-openapi.yml
- filename: famulor-io-knowledge-bases-api-openapi.yml
  format: yaml
  label: Famulor Knowledge Bases API
  slug: famulor-io-knowledge-bases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-knowledge-bases-api-openapi.yml
- filename: famulor-io-labels-api-openapi.yml
  format: yaml
  label: Famulor Labels API
  slug: famulor-io-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-labels-api-openapi.yml
- filename: famulor-io-leads-api-openapi.yml
  format: yaml
  label: Famulor Leads API
  slug: famulor-io-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-leads-api-openapi.yml
- filename: famulor-io-mid-call-tools-api-openapi.yml
  format: yaml
  label: Famulor Mid-Call Tools API
  slug: famulor-io-mid-call-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-mid-call-tools-api-openapi.yml
- filename: famulor-io-phone-numbers-api-openapi.yml
  format: yaml
  label: Famulor Phone Numbers API
  slug: famulor-io-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-phone-numbers-api-openapi.yml
- filename: famulor-io-sip-trunks-api-openapi.yml
  format: yaml
  label: Famulor SIP Trunks API
  slug: famulor-io-sip-trunks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-sip-trunks-api-openapi.yml
- filename: famulor-io-sms-api-openapi.yml
  format: yaml
  label: Famulor SMS API
  slug: famulor-io-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-sms-api-openapi.yml
- filename: famulor-io-webhooks-api-openapi.yml
  format: yaml
  label: Famulor Webhooks API
  slug: famulor-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-webhooks-api-openapi.yml
- filename: famulor-io-whats-app-api-openapi.yml
  format: yaml
  label: Famulor Whats App API
  slug: famulor-io-whats-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/famulor-io/openapi/famulor-io-whats-app-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Famulor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Famulor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Famulor
provider_slug: famulor-io
scheme_count: 1
schemes:
- description: 'API-Key als Bearer-Token: `Authorization: Bearer YOUR_API_KEY`. Key erstellen unter https://app.famulor.de.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/famulor-io-openapi.json
  type: http
slug: famulor-io-authentication
source_filename: famulor-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/famulor-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'API-Key als Bearer-Token: `Authorization: Bearer YOUR_API_KEY`. Key erstellen\n    unter https://app.famulor.de.'\n  sources:\n  - openapi/famulor-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/famulor-io/authentication/famulor-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Voice
- Telephony
- No-Code
- GDPR
---
