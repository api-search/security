---
anonymous_access: false
api_key_in: []
api_specs:
- filename: justblogged-com-api-keys-api-openapi.yml
  format: yaml
  label: JustBlogged API Keys API
  slug: justblogged-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justblogged-com/openapi/justblogged-com-api-keys-api-openapi.yml
- filename: justblogged-com-blogs-api-openapi.yml
  format: yaml
  label: JustBlogged Blogs API
  slug: justblogged-com-blogs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justblogged-com/openapi/justblogged-com-blogs-api-openapi.yml
- filename: justblogged-com-collections-api-openapi.yml
  format: yaml
  label: JustBlogged Collections API
  slug: justblogged-com-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justblogged-com/openapi/justblogged-com-collections-api-openapi.yml
- filename: justblogged-com-images-api-openapi.yml
  format: yaml
  label: JustBlogged Images API
  slug: justblogged-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justblogged-com/openapi/justblogged-com-images-api-openapi.yml
- filename: justblogged-com-members-api-openapi.yml
  format: yaml
  label: JustBlogged Members API
  slug: justblogged-com-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justblogged-com/openapi/justblogged-com-members-api-openapi.yml
- filename: justblogged-com-pages-api-openapi.yml
  format: yaml
  label: JustBlogged Pages API
  slug: justblogged-com-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justblogged-com/openapi/justblogged-com-pages-api-openapi.yml
- filename: justblogged-com-posts-api-openapi.yml
  format: yaml
  label: JustBlogged Posts API
  slug: justblogged-com-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justblogged-com/openapi/justblogged-com-posts-api-openapi.yml
- filename: justblogged-com-redirects-api-openapi.yml
  format: yaml
  label: JustBlogged Redirects API
  slug: justblogged-com-redirects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justblogged-com/openapi/justblogged-com-redirects-api-openapi.yml
- filename: justblogged-com-tags-api-openapi.yml
  format: yaml
  label: JustBlogged Tags API
  slug: justblogged-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justblogged-com/openapi/justblogged-com-tags-api-openapi.yml
- filename: justblogged-com-themes-api-openapi.yml
  format: yaml
  label: JustBlogged Themes API
  slug: justblogged-com-themes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justblogged-com/openapi/justblogged-com-themes-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: JustBlogged Authentication
name_suffix: Authentication
oauth_flows: []
overview: JustBlogged secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JustBlogged
provider_slug: justblogged-com
scheme_count: 1
schemes:
- description: 'API key authentication (format: jb_xxxx). Blog-scoped keys can manage only their bound blog and inherit the key owner''s current account status and blog permissions.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/justblogged-com-openapi.yml
  type: http
slug: justblogged-com-authentication
source_filename: justblogged-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/justblogged-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key authentication (format: jb_xxxx). Blog-scoped keys can manage only their\n    bound blog and inherit the key owner''s current account status and blog permissions.'\n  sources:\n  - openapi/justblogged-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/justblogged-com/authentication/justblogged-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Blogging
- Platform
- Free
- CustomDomain
- Software-as-a-Service
---
