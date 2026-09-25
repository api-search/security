---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datacite-activities-api-openapi.yml
  format: yaml
  label: DataCite Activities API
  slug: datacite-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-activities-api-openapi.yml
- filename: datacite-client-prefixes-api-openapi.yml
  format: yaml
  label: DataCite Client Prefixes API
  slug: datacite-client-prefixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-client-prefixes-api-openapi.yml
- filename: datacite-clients-api-openapi.yml
  format: yaml
  label: DataCite Clients API
  slug: datacite-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-clients-api-openapi.yml
- filename: datacite-events-api-openapi.yml
  format: yaml
  label: DataCite Events API
  slug: datacite-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-events-api-openapi.yml
- filename: datacite-heartbeat-api-openapi.yml
  format: yaml
  label: DataCite Heartbeat API
  slug: datacite-heartbeat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-heartbeat-api-openapi.yml
- filename: datacite-prefixes-api-openapi.yml
  format: yaml
  label: DataCite Prefixes API
  slug: datacite-prefixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-prefixes-api-openapi.yml
- filename: datacite-provider-prefixes-api-openapi.yml
  format: yaml
  label: DataCite Provider Prefixes API
  slug: datacite-provider-prefixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-provider-prefixes-api-openapi.yml
- filename: datacite-providers-api-openapi.yml
  format: yaml
  label: DataCite Providers API
  slug: datacite-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-providers-api-openapi.yml
- filename: datacite-publishers-api-openapi.yml
  format: yaml
  label: DataCite Publishers API
  slug: datacite-publishers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-publishers-api-openapi.yml
- filename: datacite-report-types-api-openapi.yml
  format: yaml
  label: DataCite Report Types API
  slug: datacite-report-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-report-types-api-openapi.yml
- filename: datacite-reports-api-openapi.yml
  format: yaml
  label: DataCite Reports API
  slug: datacite-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-reports-api-openapi.yml
- filename: datacite-repositories-api-openapi.yml
  format: yaml
  label: DataCite Repositories API
  slug: datacite-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-repositories-api-openapi.yml
- filename: datacite-status-api-openapi.yml
  format: yaml
  label: DataCite Status API
  slug: datacite-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-status-api-openapi.yml
- filename: datacite-dois-api-openapi.yml
  format: yaml
  label: DataCite Dois API
  slug: datacite-dois-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/openapi/datacite-dois-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Datacite Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataCite secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DataCite
provider_slug: datacite
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/datacite-rest-api-openapi.yml
  type: http
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/datacite-rest-api-openapi.yml
  - openapi/datacite-usage-reports-api-openapi.yml
  type: http
slug: datacite-authentication
source_filename: datacite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datacite-rest-api-openapi.yml, openapi/datacite-usage-reports-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/datacite-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/datacite-rest-api-openapi.yml\n  - openapi/datacite-usage-reports-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/authentication/datacite-authentication.yml
summary_line: http · 2 schemes
tags:
- DOI
- Persistent Identifiers
- Scholarly Metadata
- Research Data
- Open Science
- Linked Data
- DataCite
---
