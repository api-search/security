---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailinapp-com-contacts-api-openapi.yml
  format: yaml
  label: MailInApp Contacts API
  slug: mailinapp-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-contacts-api-openapi.yml
- filename: mailinapp-com-courses-api-openapi.yml
  format: yaml
  label: MailInApp Courses API
  slug: mailinapp-com-courses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-courses-api-openapi.yml
- filename: mailinapp-com-deals-api-openapi.yml
  format: yaml
  label: MailInApp Deals API
  slug: mailinapp-com-deals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-deals-api-openapi.yml
- filename: mailinapp-com-experiments-api-openapi.yml
  format: yaml
  label: MailInApp Experiments API
  slug: mailinapp-com-experiments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-experiments-api-openapi.yml
- filename: mailinapp-com-journeys-api-openapi.yml
  format: yaml
  label: MailInApp Journeys API
  slug: mailinapp-com-journeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-journeys-api-openapi.yml
- filename: mailinapp-com-live-view-api-openapi.yml
  format: yaml
  label: MailInApp Live view API
  slug: mailinapp-com-live-view-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-live-view-api-openapi.yml
- filename: mailinapp-com-send-api-openapi.yml
  format: yaml
  label: MailInApp Send API
  slug: mailinapp-com-send-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-send-api-openapi.yml
- filename: mailinapp-com-webhooks-api-openapi.yml
  format: yaml
  label: MailInApp Webhooks API
  slug: mailinapp-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-webhooks-api-openapi.yml
- filename: mailinapp-com-webinars-api-openapi.yml
  format: yaml
  label: MailInApp Webinars API
  slug: mailinapp-com-webinars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailinapp-com/openapi/mailinapp-com-webinars-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MailInApp Authentication
name_suffix: Authentication
oauth_flows: []
overview: MailInApp declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MailInApp
provider_slug: mailinapp-com
scheme_count: 1
schemes:
- evidence: 'curl -X POST https://mailinapp.com/api/v1/send \ -H "Authorization: Bearer mia_live_..." \ -H "Content-Type: application/json" \ -d ''{"to": "[email protected]", "subject": "Your one-time code", "html": "<p>Your code is 123456</p>", "text": "Your code is 123456"}'''
  how_to_obtain: Create a key under Developers in the dashboard; the full key (mia_live_...) is shown exactly once.
  name: Bearer Token
  type: http-bearer
slug: mailinapp-com-authentication
source_filename: mailinapp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mailinapp.com/docs/account/mfa
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mailinapp.com/docs/account/mfa\nsources:\n- https://mailinapp.com/docs/account/mfa\n- https://mailinapp.com/docs/getting-started/introduction\n- https://mailinapp.com/docs/getting-started/quickstart\n- https://mailinapp.com/docs/developers/quickstart\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'curl -X POST https://mailinapp.com/api/v1/send \\ -H \"Authorization: Bearer mia_live_...\" \\ -H \"Content-Type: application/json\" \\\n    -d ''{\"to\": \"[email protected]\", \"subject\": \"Your one-time code\", \"html\": \"<p>Your code is 123456</p>\", \"text\": \"Your code is 123456\"}'''\n  how_to_obtain: Create a key under Developers in the dashboard; the full key (mia_live_...) is shown exactly once.\ndocs: https://mailinapp.com/docs/account/mfa\n"
source_yaml_url: https://artifacts.apis.io/mailinapp-com/authentication/mailinapp-com-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Marketing
- Interactive
- Software-as-a-Service
---
