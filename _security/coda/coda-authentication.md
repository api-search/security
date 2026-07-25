---
api_key_in: []
api_specs:
- filename: coda-account-api-openapi.yml
  format: yaml
  label: Coda Account API
  slug: coda-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-account-api-openapi.yml
- filename: coda-analytics-api-openapi.yml
  format: yaml
  label: Coda Analytics API
  slug: coda-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-analytics-api-openapi.yml
- filename: coda-automations-api-openapi.yml
  format: yaml
  label: Coda Automations API
  slug: coda-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-automations-api-openapi.yml
- filename: coda-columns-api-openapi.yml
  format: yaml
  label: Coda Columns API
  slug: coda-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-columns-api-openapi.yml
- filename: coda-controls-api-openapi.yml
  format: yaml
  label: Coda Controls API
  slug: coda-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-controls-api-openapi.yml
- filename: coda-customdocdomains-api-openapi.yml
  format: yaml
  label: Coda CustomDocDomains API
  slug: coda-customdocdomains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-customdocdomains-api-openapi.yml
- filename: coda-docs-api-openapi.yml
  format: yaml
  label: Coda Docs API
  slug: coda-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-docs-api-openapi.yml
- filename: coda-folders-api-openapi.yml
  format: yaml
  label: Coda Folders API
  slug: coda-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-folders-api-openapi.yml
- filename: coda-formulas-api-openapi.yml
  format: yaml
  label: Coda Formulas API
  slug: coda-formulas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-formulas-api-openapi.yml
- filename: coda-go-links-api-openapi.yml
  format: yaml
  label: Coda Go Links API
  slug: coda-go-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-go-links-api-openapi.yml
- filename: coda-miscellaneous-api-openapi.yml
  format: yaml
  label: Coda Miscellaneous API
  slug: coda-miscellaneous-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-miscellaneous-api-openapi.yml
- filename: coda-packs-api-openapi.yml
  format: yaml
  label: Coda Packs API
  slug: coda-packs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-packs-api-openapi.yml
- filename: coda-pages-api-openapi.yml
  format: yaml
  label: Coda Pages API
  slug: coda-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-pages-api-openapi.yml
- filename: coda-permissions-api-openapi.yml
  format: yaml
  label: Coda Permissions API
  slug: coda-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-permissions-api-openapi.yml
- filename: coda-publishing-api-openapi.yml
  format: yaml
  label: Coda Publishing API
  slug: coda-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-publishing-api-openapi.yml
- filename: coda-rows-api-openapi.yml
  format: yaml
  label: Coda Rows API
  slug: coda-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-rows-api-openapi.yml
- filename: coda-tables-api-openapi.yml
  format: yaml
  label: Coda Tables API
  slug: coda-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-tables-api-openapi.yml
- filename: coda-workspaces-api-openapi.yml
  format: yaml
  label: Coda Workspaces API
  slug: coda-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/openapi/coda-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Coda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coda
provider_slug: coda
scheme_count: 1
schemes:
- bearerFormat: UUID
  description: 'The Coda API can be accessed using an API token, which can be obtained from [*My account*](https://coda.io/account)

    in Coda. This token should be specified by setting a header as follows.


    ```Authorization: Bearer <api_token>```


    Keep your token safe, as anyone who gets access to it can access your account. Once a token is created

    it cannot be viewed or modified, so don''t lose it.


    If you''re logge'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/coda-openapi.json
  type: http
slug: coda-authentication
source_filename: coda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coda-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: UUID\n  description: |-\n    The Coda API can be accessed using an API token, which can be obtained from [*My account*](https://coda.io/account)\n    in Coda. This token should be specified by setting a header as follows.\n\n    ```Authorization: Bearer <api_token>```\n\n    Keep your token safe, as anyone who gets access to it can access your account. Once a token is created\n    it cannot be viewed or modified, so don't lose it.\n\n    If you're logge\n  sources:\n  - openapi/coda-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coda/refs/heads/main/authentication/coda-authentication.yml
summary_line: http · 1 scheme
tags:
- Productivity
- Docs
- No-Code
- Collaboration
- Database
---
