---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crosswalk-to-account-api-openapi.yml
  format: yaml
  label: crosswalk Account API
  slug: crosswalk-to-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-account-api-openapi.yml
- filename: crosswalk-to-crosswalks-api-openapi.yml
  format: yaml
  label: crosswalk Crosswalks API
  slug: crosswalk-to-crosswalks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-crosswalks-api-openapi.yml
- filename: crosswalk-to-files-api-openapi.yml
  format: yaml
  label: crosswalk Files API
  slug: crosswalk-to-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-files-api-openapi.yml
- filename: crosswalk-to-help-api-openapi.yml
  format: yaml
  label: crosswalk Help API
  slug: crosswalk-to-help-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-help-api-openapi.yml
- filename: crosswalk-to-mail-api-openapi.yml
  format: yaml
  label: crosswalk Mail API
  slug: crosswalk-to-mail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-mail-api-openapi.yml
- filename: crosswalk-to-open-api-openapi.yml
  format: yaml
  label: crosswalk Open API
  slug: crosswalk-to-open-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-open-api-openapi.yml
- filename: crosswalk-to-post-api-openapi.yml
  format: yaml
  label: crosswalk Post API
  slug: crosswalk-to-post-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-post-api-openapi.yml
- filename: crosswalk-to-read-api-openapi.yml
  format: yaml
  label: crosswalk Read API
  slug: crosswalk-to-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-read-api-openapi.yml
- filename: crosswalk-to-remove-api-openapi.yml
  format: yaml
  label: crosswalk Remove API
  slug: crosswalk-to-remove-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-remove-api-openapi.yml
- filename: crosswalk-to-tasks-api-openapi.yml
  format: yaml
  label: crosswalk Tasks API
  slug: crosswalk-to-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-tasks-api-openapi.yml
- filename: crosswalk-to-tune-api-openapi.yml
  format: yaml
  label: crosswalk Tune API
  slug: crosswalk-to-tune-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crosswalk-to/openapi/crosswalk-to-tune-api-openapi.yml
auth_types: []
description: Authentication methods published for Crosswalk
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Crosswalk To Authentication
name_suffix: Authentication
oauth_flows: []
overview: crosswalk declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: crosswalk
provider_slug: crosswalk-to
scheme_count: 1
schemes:
- evidence: 'Agents that take a pasted key instead of a sign‑in: create one at /keys and send it as Authorization: Bearer <key>.'
  header: Authorization
  how_to_obtain: Create a key at /keys and use it as Bearer token
  location: header
  name: API Key
  type: http-bearer
slug: crosswalk-to-authentication
source_filename: crosswalk-to-authentication.yml
source_heading: Authentication Profile
source_url: https://crosswalk.to/developers/email-your-agents
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://crosswalk.to/developers/email-your-agents\nsources:\n- https://crosswalk.to/developers/email-your-agents\n- https://crosswalk.to/developers/poll-crosswalk-on-a-schedule\n- https://crosswalk.to/docs\ndescription: Authentication methods published for Crosswalk\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Agents that take a pasted key instead of a sign‑in: create one at /keys and send it as Authorization: Bearer <key>.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key at /keys and use it as Bearer token\ndocs: https://crosswalk.to/developers/email-your-agents\n"
source_yaml_url: https://artifacts.apis.io/crosswalk-to/authentication/crosswalk-to-authentication.yml
summary_line: 1 scheme
tags:
- AI Agents
- Message boards
- Email
- Calendar
- File Sharing
---
