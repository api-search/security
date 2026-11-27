---
anonymous_access: false
api_key_in: []
api_specs:
- filename: eztexting-com-blocks-api-openapi.yml
  format: yaml
  label: EZ Texting Blocks API
  slug: eztexting-com-blocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-blocks-api-openapi.yml
- filename: eztexting-com-contact-fields-api-openapi.yml
  format: yaml
  label: EZ Texting Contact Fields API
  slug: eztexting-com-contact-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-contact-fields-api-openapi.yml
- filename: eztexting-com-contact-groups-api-openapi.yml
  format: yaml
  label: EZ Texting Contact Groups API
  slug: eztexting-com-contact-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-contact-groups-api-openapi.yml
- filename: eztexting-com-contacts-api-openapi.yml
  format: yaml
  label: EZ Texting Contacts API
  slug: eztexting-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-contacts-api-openapi.yml
- filename: eztexting-com-conversations-api-openapi.yml
  format: yaml
  label: EZ Texting Conversations API
  slug: eztexting-com-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-conversations-api-openapi.yml
- filename: eztexting-com-credits-api-openapi.yml
  format: yaml
  label: EZ Texting Credits API
  slug: eztexting-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-credits-api-openapi.yml
- filename: eztexting-com-keywords-api-openapi.yml
  format: yaml
  label: EZ Texting Keywords API
  slug: eztexting-com-keywords-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-keywords-api-openapi.yml
- filename: eztexting-com-media-files-api-openapi.yml
  format: yaml
  label: EZ Texting Media Files API
  slug: eztexting-com-media-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-media-files-api-openapi.yml
- filename: eztexting-com-message-reports-api-openapi.yml
  format: yaml
  label: EZ Texting Message Reports API
  slug: eztexting-com-message-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-message-reports-api-openapi.yml
- filename: eztexting-com-message-templates-api-openapi.yml
  format: yaml
  label: EZ Texting Message Templates API
  slug: eztexting-com-message-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-message-templates-api-openapi.yml
- filename: eztexting-com-messages-api-openapi.yml
  format: yaml
  label: EZ Texting Messages API
  slug: eztexting-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-messages-api-openapi.yml
- filename: eztexting-com-tokens-api-openapi.yml
  format: yaml
  label: EZ Texting Tokens API
  slug: eztexting-com-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-tokens-api-openapi.yml
- filename: eztexting-com-webhooks-api-openapi.yml
  format: yaml
  label: EZ Texting Webhooks API
  slug: eztexting-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eztexting-com/openapi/eztexting-com-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: EZ Texting Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: EZ Texting secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: EZ Texting
provider_slug: eztexting-com
scheme_count: 2
schemes:
- name: basic_auth
  scheme: basic
  sources:
  - openapi/eztexting-com-api-openapi.yml
  type: http
- flows:
  - flow: password
    scopes: 2
    tokenUrl: http://nova-app.stg0.cf.wtf/oauth_token/generate/swagger
  name: oauth_auth
  sources:
  - openapi/eztexting-com-api-openapi.yml
  type: oauth2
slug: eztexting-com-authentication
source_filename: eztexting-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/eztexting-com-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/eztexting-com-api-openapi.yml\n- name: oauth_auth\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: http://nova-app.stg0.cf.wtf/oauth_token/generate/swagger\n    scopes: 2\n  sources:\n  - openapi/eztexting-com-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/eztexting-com/authentication/eztexting-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- SMS
- Marketing
- Communications
- Text Messaging
---
