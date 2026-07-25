---
api_key_in: []
api_specs:
- filename: simpletexting-campaigns-api-openapi.yml
  format: yaml
  label: SimpleTexting Campaigns API
  slug: simpletexting-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-campaigns-api-openapi.yml
- filename: simpletexting-contact-lists-api-openapi.yml
  format: yaml
  label: SimpleTexting Contact Lists API
  slug: simpletexting-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-contact-lists-api-openapi.yml
- filename: simpletexting-contact-segments-api-openapi.yml
  format: yaml
  label: SimpleTexting Contact Segments API
  slug: simpletexting-contact-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-contact-segments-api-openapi.yml
- filename: simpletexting-contacts-api-openapi.yml
  format: yaml
  label: SimpleTexting Contacts API
  slug: simpletexting-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-contacts-api-openapi.yml
- filename: simpletexting-contacts-batch-operations-api-openapi.yml
  format: yaml
  label: SimpleTexting Contacts - Batch Operations API
  slug: simpletexting-contacts-batch-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-contacts-batch-operations-api-openapi.yml
- filename: simpletexting-custom-fields-api-openapi.yml
  format: yaml
  label: SimpleTexting Custom Fields API
  slug: simpletexting-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-custom-fields-api-openapi.yml
- filename: simpletexting-media-items-api-openapi.yml
  format: yaml
  label: SimpleTexting Media Items API
  slug: simpletexting-media-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-media-items-api-openapi.yml
- filename: simpletexting-messages-api-openapi.yml
  format: yaml
  label: SimpleTexting Messages API
  slug: simpletexting-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-messages-api-openapi.yml
- filename: simpletexting-tenant-api-openapi.yml
  format: yaml
  label: SimpleTexting Tenant API
  slug: simpletexting-tenant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-tenant-api-openapi.yml
- filename: simpletexting-webhooks-api-openapi.yml
  format: yaml
  label: SimpleTexting Webhooks API
  slug: simpletexting-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/openapi/simpletexting-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Simpletexting Authentication
name_suffix: Authentication
oauth_flows: []
overview: SimpleTexting secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SimpleTexting
provider_slug: simpletexting
scheme_count: 1
schemes:
- description: 'Send the API token as a bearer token in the Authorization header: `Authorization: Bearer <token>`. Generate a token in the SimpleTexting web app under Settings.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/simpletexting-openapi.yml
  type: http
slug: simpletexting-authentication
source_filename: simpletexting-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/simpletexting-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Send the API token as a bearer token in the Authorization header: `Authorization:\n    Bearer <token>`. Generate a token in the SimpleTexting web app under Settings.'\n  sources:\n  - openapi/simpletexting-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpletexting/refs/heads/main/authentication/simpletexting-authentication.yml
summary_line: http · 1 scheme
tags:
- SMS
- MMS
- Messaging
- Marketing
- Text Messaging
---
