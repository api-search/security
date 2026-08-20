---
api_key_in:
- header
api_specs:
- filename: convoy-delivery-attempts-api-openapi.yml
  format: yaml
  label: Convoy Delivery Attempts API
  slug: convoy-delivery-attempts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-delivery-attempts-api-openapi.yml
- filename: convoy-endpoints-api-openapi.yml
  format: yaml
  label: Convoy Endpoints API
  slug: convoy-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-endpoints-api-openapi.yml
- filename: convoy-event-deliveries-api-openapi.yml
  format: yaml
  label: Convoy Event Deliveries API
  slug: convoy-event-deliveries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-event-deliveries-api-openapi.yml
- filename: convoy-events-api-openapi.yml
  format: yaml
  label: Convoy Events API
  slug: convoy-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-events-api-openapi.yml
- filename: convoy-eventtypes-api-openapi.yml
  format: yaml
  label: Convoy EventTypes API
  slug: convoy-eventtypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-eventtypes-api-openapi.yml
- filename: convoy-filters-api-openapi.yml
  format: yaml
  label: Convoy Filters API
  slug: convoy-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-filters-api-openapi.yml
- filename: convoy-meta-events-api-openapi.yml
  format: yaml
  label: Convoy Meta Events API
  slug: convoy-meta-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-meta-events-api-openapi.yml
- filename: convoy-onboard-api-openapi.yml
  format: yaml
  label: Convoy Onboard API
  slug: convoy-onboard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-onboard-api-openapi.yml
- filename: convoy-portal-links-api-openapi.yml
  format: yaml
  label: Convoy Portal Links API
  slug: convoy-portal-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-portal-links-api-openapi.yml
- filename: convoy-sources-api-openapi.yml
  format: yaml
  label: Convoy Sources API
  slug: convoy-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-sources-api-openapi.yml
- filename: convoy-subscriptions-api-openapi.yml
  format: yaml
  label: Convoy Subscriptions API
  slug: convoy-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/openapi/convoy-subscriptions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Convoy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convoy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Convoy
provider_slug: convoy
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/convoy-openapi.yml
  type: apiKey
slug: convoy-authentication
source_filename: convoy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/convoy-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/convoy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convoy/refs/heads/main/authentication/convoy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Webhook
- Webhook Gateway
- Event Delivery
- Eventing
- Messaging
- Integration
- API Infrastructure
---
