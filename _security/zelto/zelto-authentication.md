---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zelto-action-checks-api-openapi.yml
  format: yaml
  label: Zelto Action checks API
  slug: zelto-action-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-action-checks-api-openapi.yml
- filename: zelto-agents-api-openapi.yml
  format: yaml
  label: Zelto Agents API
  slug: zelto-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-agents-api-openapi.yml
- filename: zelto-buckets-api-openapi.yml
  format: yaml
  label: Zelto Buckets API
  slug: zelto-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-buckets-api-openapi.yml
- filename: zelto-companies-api-openapi.yml
  format: yaml
  label: Zelto Companies API
  slug: zelto-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-companies-api-openapi.yml
- filename: zelto-conversations-api-openapi.yml
  format: yaml
  label: Zelto Conversations API
  slug: zelto-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-conversations-api-openapi.yml
- filename: zelto-customer-metrics-api-openapi.yml
  format: yaml
  label: Zelto Customer Metrics API
  slug: zelto-customer-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-customer-metrics-api-openapi.yml
- filename: zelto-experiments-api-openapi.yml
  format: yaml
  label: Zelto Experiments API
  slug: zelto-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-experiments-api-openapi.yml
- filename: zelto-findings-api-openapi.yml
  format: yaml
  label: Zelto Findings API
  slug: zelto-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-findings-api-openapi.yml
- filename: zelto-organizations-api-openapi.yml
  format: yaml
  label: Zelto Organizations API
  slug: zelto-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-organizations-api-openapi.yml
- filename: zelto-reports-api-openapi.yml
  format: yaml
  label: Zelto Reports API
  slug: zelto-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-reports-api-openapi.yml
- filename: zelto-reviews-api-openapi.yml
  format: yaml
  label: Zelto Reviews API
  slug: zelto-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/openapi/zelto-reviews-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Zelto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zelto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zelto
provider_slug: zelto
scheme_count: 1
schemes:
- description: 'Send `Authorization: Bearer YOUR_API_KEY`. The key resolves to a single organization.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/zelto-openapi.json
  type: http
slug: zelto-authentication
source_filename: zelto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: derived\nsource: openapi/zelto-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Send `Authorization: Bearer YOUR_API_KEY`. The key resolves to a single organization.'\n  sources:\n  - openapi/zelto-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zelto/refs/heads/main/authentication/zelto-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- VoiceAI
- QA
- Production
- Analytics
- Monitoring
---
