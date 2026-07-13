---
api_key_in: []
api_specs:
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Customers API
  slug: pushpress-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Check-Ins API
  slug: pushpress-checkins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Appointments API
  slug: pushpress-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Classes API
  slug: pushpress-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Events API
  slug: pushpress-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Enrollments and Plans API
  slug: pushpress-enrollments-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Company API
  slug: pushpress-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Invitations API
  slug: pushpress-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Messaging API
  slug: pushpress-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress Webhooks API
  slug: pushpress-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
- filename: pushpress-openapi.yml
  format: yaml
  label: PushPress API Keys API
  slug: pushpress-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/openapi/pushpress-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pushpress Authentication
name_suffix: Authentication
oauth_flows: []
overview: PushPress secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PushPress
provider_slug: pushpress
scheme_count: 1
schemes:
- description: API key issued in the PushPress developer portal (developer.pushpress.com), passed in the `API-KEY` request header. Keys can also be created, listed, retrieved, and revoked programmatically via the /keys endpoints. Every request is additionally scoped to a single gym location with a `company-id` header.
  in: header
  name: api_key
  parameterName: API-KEY
  sources:
  - openapi/pushpress-openapi.yml
  - https://github.com/PushPress/pushpress-ts
  type: apiKey
slug: pushpress-authentication
source_filename: pushpress-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: openapi/pushpress-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameterName: API-KEY\n  description: >-\n    API key issued in the PushPress developer portal (developer.pushpress.com),\n    passed in the `API-KEY` request header. Keys can also be created, listed,\n    retrieved, and revoked programmatically via the /keys endpoints. Every\n    request is additionally scoped to a single gym location with a `company-id`\n    header.\n  sources:\n  - openapi/pushpress-openapi.yml\n  - https://github.com/PushPress/pushpress-ts\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pushpress/refs/heads/main/authentication/pushpress-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fitness
- Gym Management
- Membership Management
- Fitness Software
- Class Scheduling
- Billing
- CRM
- Wellness
- SaaS
- Webhooks
---
