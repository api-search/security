---
anonymous_access: false
api_key_in: []
api_specs:
- filename: meibo-io-entries-api-openapi.yml
  format: yaml
  label: meibo Entries API
  slug: meibo-io-entries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meibo-io/openapi/meibo-io-entries-api-openapi.yml
- filename: meibo-io-invites-api-openapi.yml
  format: yaml
  label: meibo Invites API
  slug: meibo-io-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meibo-io/openapi/meibo-io-invites-api-openapi.yml
- filename: meibo-io-moderation-api-openapi.yml
  format: yaml
  label: meibo Moderation API
  slug: meibo-io-moderation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meibo-io/openapi/meibo-io-moderation-api-openapi.yml
- filename: meibo-io-settings-api-openapi.yml
  format: yaml
  label: meibo Settings API
  slug: meibo-io-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meibo-io/openapi/meibo-io-settings-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: meibo Authentication
name_suffix: Authentication
oauth_flows: []
overview: meibo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: meibo
provider_slug: meibo-io
scheme_count: 1
schemes:
- description: 'The key, sent as `Authorization: Bearer <key>`. The `Bearer ` prefix may

    be left off. A key that is missing, revoked or expired gets `401`, and

    so does a key made for one directory, before keys reached every

    directory, once that directory has changed hands.


    A key holds some of these scopes, chosen by the owner when it is made.

    Each operation''s `security` names the scopes it needs, and an operatio'
  name: directoryKey
  scheme: bearer
  sources:
  - openapi/meibo-io-openapi.yml
  type: http
slug: meibo-io-authentication
source_filename: meibo-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/meibo-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: directoryKey\n  type: http\n  scheme: bearer\n  description: |-\n    The key, sent as `Authorization: Bearer <key>`. The `Bearer ` prefix may\n    be left off. A key that is missing, revoked or expired gets `401`, and\n    so does a key made for one directory, before keys reached every\n    directory, once that directory has changed hands.\n\n    A key holds some of these scopes, chosen by the owner when it is made.\n    Each operation's `security` names the scopes it needs, and an operatio\n  sources:\n  - openapi/meibo-io-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/meibo-io/authentication/meibo-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- Directory
- Privacy
- Software-as-a-Service
- Schools
---
