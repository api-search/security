---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: customermates-com-addresses-api-openapi.yml
  format: yaml
  label: Customermates Addresses API
  slug: customermates-com-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-addresses-api-openapi.yml
- filename: customermates-com-data-views-api-openapi.yml
  format: yaml
  label: Customermates Data Views API
  slug: customermates-com-data-views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-data-views-api-openapi.yml
- filename: customermates-com-files-api-openapi.yml
  format: yaml
  label: Customermates Files API
  slug: customermates-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-files-api-openapi.yml
- filename: customermates-com-knowledge-base-api-openapi.yml
  format: yaml
  label: Customermates Knowledge Base API
  slug: customermates-com-knowledge-base-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-knowledge-base-api-openapi.yml
- filename: customermates-com-members-api-openapi.yml
  format: yaml
  label: Customermates Members API
  slug: customermates-com-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-members-api-openapi.yml
- filename: customermates-com-messaging-api-openapi.yml
  format: yaml
  label: Customermates Messaging API
  slug: customermates-com-messaging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-messaging-api-openapi.yml
- filename: customermates-com-operations-api-openapi.yml
  format: yaml
  label: Customermates Operations API
  slug: customermates-com-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-operations-api-openapi.yml
- filename: customermates-com-record-links-api-openapi.yml
  format: yaml
  label: Customermates Record Links API
  slug: customermates-com-record-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-record-links-api-openapi.yml
- filename: customermates-com-records-api-openapi.yml
  format: yaml
  label: Customermates Records API
  slug: customermates-com-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-records-api-openapi.yml
- filename: customermates-com-roles-api-openapi.yml
  format: yaml
  label: Customermates Roles API
  slug: customermates-com-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-roles-api-openapi.yml
- filename: customermates-com-routines-api-openapi.yml
  format: yaml
  label: Customermates Routines API
  slug: customermates-com-routines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-routines-api-openapi.yml
- filename: customermates-com-trash-api-openapi.yml
  format: yaml
  label: Customermates Trash API
  slug: customermates-com-trash-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-trash-api-openapi.yml
- filename: customermates-com-users-api-openapi.yml
  format: yaml
  label: Customermates Users API
  slug: customermates-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-users-api-openapi.yml
- filename: customermates-com-webhooks-api-openapi.yml
  format: yaml
  label: Customermates Webhooks API
  slug: customermates-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-webhooks-api-openapi.yml
- filename: customermates-com-widgets-api-openapi.yml
  format: yaml
  label: Customermates Widgets API
  slug: customermates-com-widgets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/customermates-com/openapi/customermates-com-widgets-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Customermates Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Customermates secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Customermates
provider_slug: customermates-com
scheme_count: 2
schemes:
- description: API key authentication. Create an API key in your user profile and include it in the x-api-key header.
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/customermates-openapi.json
  type: apiKey
- description: Signed token of one file, part of an upload URL or a downloadUrl. It acts for the person who requested it for 15 minutes.
  in: query
  name: fileLinkToken
  parameter: token
  sources:
  - openapi/customermates-openapi.json
  type: apiKey
slug: customermates-com-authentication
source_filename: customermates-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: derived\nsource: openapi/customermates-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key authentication. Create an API key in your user profile and include it\n    in the x-api-key header.\n  sources:\n  - openapi/customermates-openapi.json\n- name: fileLinkToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Signed token of one file, part of an upload URL or a downloadUrl. It acts for\n    the person who requested it for 15 minutes.\n  sources:\n  - openapi/customermates-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/customermates-com/authentication/customermates-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- CRM
- Open-Source
- AI
- SaaS
---
