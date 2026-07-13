---
api_key_in: []
api_specs:
- filename: hookdeck-connections-api-openapi.yml
  format: yaml
  label: Hookdeck Connections API
  slug: hookdeck-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-connections-api-openapi.yml
- filename: hookdeck-sources-api-openapi.yml
  format: yaml
  label: Hookdeck Sources API
  slug: hookdeck-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-sources-api-openapi.yml
- filename: hookdeck-destinations-api-openapi.yml
  format: yaml
  label: Hookdeck Destinations API
  slug: hookdeck-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-destinations-api-openapi.yml
- filename: hookdeck-events-api-openapi.yml
  format: yaml
  label: Hookdeck Events API
  slug: hookdeck-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-events-api-openapi.yml
- filename: hookdeck-requests-api-openapi.yml
  format: yaml
  label: Hookdeck Requests API
  slug: hookdeck-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-requests-api-openapi.yml
- filename: hookdeck-transformations-api-openapi.yml
  format: yaml
  label: Hookdeck Transformations API
  slug: hookdeck-transformations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-transformations-api-openapi.yml
- filename: hookdeck-bookmarks-api-openapi.yml
  format: yaml
  label: Hookdeck Bookmarks API
  slug: hookdeck-bookmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-bookmarks-api-openapi.yml
- filename: hookdeck-bulk-operations-api-openapi.yml
  format: yaml
  label: Hookdeck Bulk Operations API
  slug: hookdeck-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-bulk-operations-api-openapi.yml
- filename: hookdeck-issues-api-openapi.yml
  format: yaml
  label: Hookdeck Issues API
  slug: hookdeck-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-issues-api-openapi.yml
- filename: hookdeck-metrics-api-openapi.yml
  format: yaml
  label: Hookdeck Metrics API
  slug: hookdeck-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-metrics-api-openapi.yml
- filename: hookdeck-integrations-api-openapi.yml
  format: yaml
  label: Hookdeck Integrations API
  slug: hookdeck-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-integrations-api-openapi.yml
- filename: hookdeck-notifications-api-openapi.yml
  format: yaml
  label: Hookdeck Notifications API
  slug: hookdeck-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/openapi/hookdeck-notifications-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hookdeck Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hookdeck secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hookdeck
provider_slug: hookdeck
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hookdeck-bookmarks-api-openapi.yml
  - openapi/hookdeck-bulk-operations-api-openapi.yml
  - openapi/hookdeck-connections-api-openapi.yml
  - openapi/hookdeck-destinations-api-openapi.yml
  - openapi/hookdeck-events-api-openapi.yml
  - openapi/hookdeck-integrations-api-openapi.yml
  - openapi/hookdeck-issues-api-openapi.yml
  - openapi/hookdeck-metrics-api-openapi.yml
  - openapi/hookdeck-notifications-api-openapi.yml
  - openapi/hookdeck-requests-api-openapi.yml
  - openapi/hookdeck-sources-api-openapi.yml
  - openapi/hookdeck-transformations-api-openapi.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/hookdeck-bookmarks-api-openapi.yml
  - openapi/hookdeck-bulk-operations-api-openapi.yml
  - openapi/hookdeck-connections-api-openapi.yml
  - openapi/hookdeck-destinations-api-openapi.yml
  - openapi/hookdeck-events-api-openapi.yml
  - openapi/hookdeck-integrations-api-openapi.yml
  - openapi/hookdeck-issues-api-openapi.yml
  - openapi/hookdeck-metrics-api-openapi.yml
  - openapi/hookdeck-notifications-api-openapi.yml
  - openapi/hookdeck-requests-api-openapi.yml
  - openapi/hookdeck-sources-api-openapi.yml
  - openapi/hookdeck-transformations-api-openapi.yml
  type: http
slug: hookdeck-authentication
source_filename: hookdeck-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hookdeck-bookmarks-api-openapi.yml, openapi/hookdeck-bulk-operations-api-openapi.yml,\n  openapi/hookdeck-connections-api-openapi.yml, openapi/hookdeck-destinations-api-openapi.yml,\n  openapi/hookdeck-events-api-openapi.yml, openapi/hookdeck-integrations-api-openapi.yml, openapi/hookdeck-issues-api-openapi.yml,\n  openapi/hookdeck-metrics-api-openapi.yml, openapi/hookdeck-notifications-api-openapi.yml,\n  openapi/hookdeck-requests-api-openapi.yml, openapi/hookdeck-sources-api-openapi.yml, openapi/hookdeck-transformations-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hookdeck-bookmarks-api-openapi.yml\n  - openapi/hookdeck-bulk-operations-api-openapi.yml\n  - openapi/hookdeck-connections-api-openapi.yml\n  - openapi/hookdeck-destinations-api-openapi.yml\n  - openapi/hookdeck-events-api-openapi.yml\n  - openapi/hookdeck-integrations-api-openapi.yml\n\
  \  - openapi/hookdeck-issues-api-openapi.yml\n  - openapi/hookdeck-metrics-api-openapi.yml\n  - openapi/hookdeck-notifications-api-openapi.yml\n  - openapi/hookdeck-requests-api-openapi.yml\n  - openapi/hookdeck-sources-api-openapi.yml\n  - openapi/hookdeck-transformations-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/hookdeck-bookmarks-api-openapi.yml\n  - openapi/hookdeck-bulk-operations-api-openapi.yml\n  - openapi/hookdeck-connections-api-openapi.yml\n  - openapi/hookdeck-destinations-api-openapi.yml\n  - openapi/hookdeck-events-api-openapi.yml\n  - openapi/hookdeck-integrations-api-openapi.yml\n  - openapi/hookdeck-issues-api-openapi.yml\n  - openapi/hookdeck-metrics-api-openapi.yml\n  - openapi/hookdeck-notifications-api-openapi.yml\n  - openapi/hookdeck-requests-api-openapi.yml\n  - openapi/hookdeck-sources-api-openapi.yml\n  - openapi/hookdeck-transformations-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hookdeck/refs/heads/main/authentication/hookdeck-authentication.yml
summary_line: http · 2 schemes
tags:
- Webhooks
- Event Gateways
- Gateways
- Events
- Event Infrastructure
- Event-Driven
- Messaging
- Queues
- Retries
- Transformations
- Observability
---
