---
api_key_in: []
api_specs:
- filename: inflammatix-categories-api-openapi.yml
  format: yaml
  label: Inflammatix Categories API
  slug: inflammatix-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-categories-api-openapi.yml
- filename: inflammatix-comments-api-openapi.yml
  format: yaml
  label: Inflammatix Comments API
  slug: inflammatix-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-comments-api-openapi.yml
- filename: inflammatix-coursecategories-api-openapi.yml
  format: yaml
  label: Inflammatix Course Categories API
  slug: inflammatix-coursecategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-coursecategories-api-openapi.yml
- filename: inflammatix-courses-api-openapi.yml
  format: yaml
  label: Inflammatix Courses API
  slug: inflammatix-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-courses-api-openapi.yml
- filename: inflammatix-coursetags-api-openapi.yml
  format: yaml
  label: Inflammatix Course Tags API
  slug: inflammatix-coursetags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-coursetags-api-openapi.yml
- filename: inflammatix-lessons-api-openapi.yml
  format: yaml
  label: Inflammatix Lessons API
  slug: inflammatix-lessons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-lessons-api-openapi.yml
- filename: inflammatix-media-api-openapi.yml
  format: yaml
  label: Inflammatix Media API
  slug: inflammatix-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-media-api-openapi.yml
- filename: inflammatix-pages-api-openapi.yml
  format: yaml
  label: Inflammatix Pages API
  slug: inflammatix-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-pages-api-openapi.yml
- filename: inflammatix-posts-api-openapi.yml
  format: yaml
  label: Inflammatix Posts API
  slug: inflammatix-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-posts-api-openapi.yml
- filename: inflammatix-publicationcategories-api-openapi.yml
  format: yaml
  label: Inflammatix Publication Categories API
  slug: inflammatix-publicationcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-publicationcategories-api-openapi.yml
- filename: inflammatix-publications-api-openapi.yml
  format: yaml
  label: Inflammatix Publications API
  slug: inflammatix-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-publications-api-openapi.yml
- filename: inflammatix-quizzes-api-openapi.yml
  format: yaml
  label: Inflammatix Quizzes API
  slug: inflammatix-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-quizzes-api-openapi.yml
- filename: inflammatix-search-api-openapi.yml
  format: yaml
  label: Inflammatix Search API
  slug: inflammatix-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-search-api-openapi.yml
- filename: inflammatix-statuses-api-openapi.yml
  format: yaml
  label: Inflammatix Statuses API
  slug: inflammatix-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-statuses-api-openapi.yml
- filename: inflammatix-tags-api-openapi.yml
  format: yaml
  label: Inflammatix Tags API
  slug: inflammatix-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-tags-api-openapi.yml
- filename: inflammatix-taxonomies-api-openapi.yml
  format: yaml
  label: Inflammatix Taxonomies API
  slug: inflammatix-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-taxonomies-api-openapi.yml
- filename: inflammatix-types-api-openapi.yml
  format: yaml
  label: Inflammatix Types API
  slug: inflammatix-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-types-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Inflammatix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inflammatix secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Inflammatix
provider_slug: inflammatix
scheme_count: 1
schemes:
- description: WordPress Application Passwords, advertised by the site's own REST index (authentication.application-passwords.endpoints.authorization = https://inflammatix.com/wp-admin/authorize-application.php). Required only for write operations and non-public collections; the operations modelled here are anonymously readable.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/inflammatix-content-openapi.yml
  - openapi/inflammatix-support-content-openapi.yml
  type: http
slug: inflammatix-authentication
source_filename: inflammatix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: derived\nsource: openapi/inflammatix-content-openapi.yml, openapi/inflammatix-support-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords, advertised by the site's own REST index (authentication.application-passwords.endpoints.authorization\n    = https://inflammatix.com/wp-admin/authorize-application.php). Required only for write operations\n    and non-public collections; the operations modelled here are anonymously readable.\n  sources:\n  - openapi/inflammatix-content-openapi.yml\n  - openapi/inflammatix-support-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/authentication/inflammatix-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Health
- Healthcare
- Diagnostics
- Medical Devices
- In Vitro Diagnostics
- Molecular Diagnostics
- Sepsis
- Machine-Learning
- Life Sciences
- Point of Care
- Content
---
