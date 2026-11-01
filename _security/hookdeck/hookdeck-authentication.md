---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hookdeck-connections-api-openapi.yml
  format: yaml
  label: Hookdeck Connections API
  slug: hookdeck-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-connections-api-openapi.yml
- filename: hookdeck-sources-api-openapi.yml
  format: yaml
  label: Hookdeck Sources API
  slug: hookdeck-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-sources-api-openapi.yml
- filename: hookdeck-destinations-api-openapi.yml
  format: yaml
  label: Hookdeck Destinations API
  slug: hookdeck-destinations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-destinations-api-openapi.yml
- filename: hookdeck-events-api-openapi.yml
  format: yaml
  label: Hookdeck Events API
  slug: hookdeck-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-events-api-openapi.yml
- filename: hookdeck-requests-api-openapi.yml
  format: yaml
  label: Hookdeck Requests API
  slug: hookdeck-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-requests-api-openapi.yml
- filename: hookdeck-transformations-api-openapi.yml
  format: yaml
  label: Hookdeck Transformations API
  slug: hookdeck-transformations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-transformations-api-openapi.yml
- filename: hookdeck-bookmarks-api-openapi.yml
  format: yaml
  label: Hookdeck Bookmarks API
  slug: hookdeck-bookmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-bookmarks-api-openapi.yml
- filename: hookdeck-issues-api-openapi.yml
  format: yaml
  label: Hookdeck Issues API
  slug: hookdeck-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-issues-api-openapi.yml
- filename: hookdeck-metrics-api-openapi.yml
  format: yaml
  label: Hookdeck Metrics API
  slug: hookdeck-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-metrics-api-openapi.yml
- filename: hookdeck-integrations-api-openapi.yml
  format: yaml
  label: Hookdeck Integrations API
  slug: hookdeck-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-integrations-api-openapi.yml
- filename: hookdeck-notifications-api-openapi.yml
  format: yaml
  label: Hookdeck Notifications API
  slug: hookdeck-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-notifications-api-openapi.yml
- filename: hookdeck-attempts-api-openapi.yml
  format: yaml
  label: Hookdeck Attempts API
  slug: hookdeck-attempts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-attempts-api-openapi.yml
- filename: hookdeck-issue-triggers-api-openapi.yml
  format: yaml
  label: Hookdeck Issue Triggers API
  slug: hookdeck-issue-triggers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-issue-triggers-api-openapi.yml
- filename: hookdeck-configuration-api-openapi.yml
  format: yaml
  label: Hookdeck Configuration API
  slug: hookdeck-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-configuration-api-openapi.yml
- filename: hookdeck-health-api-openapi.yml
  format: yaml
  label: Hookdeck Health API
  slug: hookdeck-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-health-api-openapi.yml
- filename: hookdeck-operator-events-api-openapi.yml
  format: yaml
  label: Hookdeck Operator Events API
  slug: hookdeck-operator-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-operator-events-api-openapi.yml
- filename: hookdeck-publish-api-openapi.yml
  format: yaml
  label: Hookdeck Publish API
  slug: hookdeck-publish-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-publish-api-openapi.yml
- filename: hookdeck-retry-api-openapi.yml
  format: yaml
  label: Hookdeck Retry API
  slug: hookdeck-retry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-retry-api-openapi.yml
- filename: hookdeck-schemas-api-openapi.yml
  format: yaml
  label: Hookdeck Schemas API
  slug: hookdeck-schemas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-schemas-api-openapi.yml
- filename: hookdeck-tenants-api-openapi.yml
  format: yaml
  label: Hookdeck Tenants API
  slug: hookdeck-tenants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-tenants-api-openapi.yml
- filename: hookdeck-topics-api-openapi.yml
  format: yaml
  label: Hookdeck Topics API
  slug: hookdeck-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hookdeck/openapi/hookdeck-topics-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
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
source_yaml_url: https://artifacts.apis.io/hookdeck/authentication/hookdeck-authentication.yml
summary_line: http · 2 schemes
tags:
- Webhook
- Event Gateways
- Gateways
- Event
- Event Infrastructure
- Event-Driven
- Messaging
- Queues
- Retries
- Transformation
- Observability
---
