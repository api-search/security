---
api_key_in:
- cookie
api_specs:
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Studio Clients & CRM API
  slug: pixieset-studio-clients-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Studio Sessions & Booking API
  slug: pixieset-studio-sessions-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Studio Invoices & Payments API
  slug: pixieset-studio-invoices-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Studio Contracts API
  slug: pixieset-studio-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Gallery Collections & Delivery API
  slug: pixieset-gallery-collections-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pixieset Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pixieset secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pixieset
provider_slug: pixieset
scheme_count: 1
schemes:
- description: Session cookie issued by the Pixieset web login flow (studio.pixieset.com/login or galleries.pixieset.com/login). This is the internal web-app session mechanism, not a published API-key or OAuth developer credential - Pixieset does not offer either for third-party use. Write operations additionally require an X-CSRF-Token header per the reverse-engineered documentation.
  in: cookie
  name: sessionCookie
  parameter: session_cookie
  sources:
  - openapi/pixieset-openapi.yml
  type: apiKey
slug: pixieset-authentication
source_filename: pixieset-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pixieset-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: session_cookie\n  description: Session cookie issued by the Pixieset web login flow (studio.pixieset.com/login\n    or galleries.pixieset.com/login). This is the internal web-app session mechanism, not a\n    published API-key or OAuth developer credential - Pixieset does not offer either for third-party\n    use. Write operations additionally require an X-CSRF-Token header per the reverse-engineered\n    documentation.\n  sources:\n  - openapi/pixieset-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/authentication/pixieset-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Photography
- Client Galleries
- Studio Management
- CRM
- Booking
- Invoicing
- Contracts
- No Public API
---
