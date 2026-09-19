---
anonymous_access: false
api_key_in: []
api_specs:
- filename: unlock-articles-api-openapi.yml
  format: yaml
  label: Unlock Articles API
  slug: unlock-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-articles-api-openapi.yml
- filename: unlock-authors-api-openapi.yml
  format: yaml
  label: Unlock Authors API
  slug: unlock-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-authors-api-openapi.yml
- filename: unlock-company-api-openapi.yml
  format: yaml
  label: Unlock Company API
  slug: unlock-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-company-api-openapi.yml
- filename: unlock-discovery-api-openapi.yml
  format: yaml
  label: Unlock Discovery API
  slug: unlock-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-discovery-api-openapi.yml
- filename: unlock-education-api-openapi.yml
  format: yaml
  label: Unlock Education API
  slug: unlock-education-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-education-api-openapi.yml
- filename: unlock-faq-api-openapi.yml
  format: yaml
  label: Unlock FAQ API
  slug: unlock-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-faq-api-openapi.yml
- filename: unlock-lessons-api-openapi.yml
  format: yaml
  label: Unlock Lessons API
  slug: unlock-lessons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-lessons-api-openapi.yml
- filename: unlock-media-api-openapi.yml
  format: yaml
  label: Unlock Media API
  slug: unlock-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-media-api-openapi.yml
- filename: unlock-navigation-api-openapi.yml
  format: yaml
  label: Unlock Navigation API
  slug: unlock-navigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-navigation-api-openapi.yml
- filename: unlock-pages-api-openapi.yml
  format: yaml
  label: Unlock Pages API
  slug: unlock-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-pages-api-openapi.yml
- filename: unlock-posts-api-openapi.yml
  format: yaml
  label: Unlock Posts API
  slug: unlock-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-posts-api-openapi.yml
- filename: unlock-search-api-openapi.yml
  format: yaml
  label: Unlock Search API
  slug: unlock-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-search-api-openapi.yml
- filename: unlock-stories-api-openapi.yml
  format: yaml
  label: Unlock Stories API
  slug: unlock-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-stories-api-openapi.yml
- filename: unlock-taxonomies-api-openapi.yml
  format: yaml
  label: Unlock Taxonomies API
  slug: unlock-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-taxonomies-api-openapi.yml
- filename: unlock-testimonials-api-openapi.yml
  format: yaml
  label: Unlock Testimonials API
  slug: unlock-testimonials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-testimonials-api-openapi.yml
- filename: unlock-topics-api-openapi.yml
  format: yaml
  label: Unlock Topics API
  slug: unlock-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-topics-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Unlock Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unlock secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Unlock
provider_slug: unlock
scheme_count: 1
schemes:
- description: WordPress application password (HTTP Basic). Advertised by this deployment at https://www.unlock.com/wp/wp-admin/authorize-application.php in the `authentication` block of the route index. It gates the write methods on these routes; every operation documented here is anonymous read and requires no credential.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/unlock-editorial-api-openapi.yml
  - openapi/unlock-site-content-api-openapi.yml
  type: http
slug: unlock-authentication
source_filename: unlock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: derived\nsource: openapi/unlock-editorial-api-openapi.yml, openapi/unlock-site-content-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application password (HTTP Basic). Advertised by this deployment at\n    https://www.unlock.com/wp/wp-admin/authorize-application.php in the `authentication` block\n    of the route index. It gates the write methods on these routes; every operation documented\n    here is anonymous read and requires no credential.\n  sources:\n  - openapi/unlock-editorial-api-openapi.yml\n  - openapi/unlock-site-content-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/authentication/unlock-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Financial-Services
- Fintech
- Home Equity
- Mortgage
- Real-Estate
- Consumer Lending
- Home Equity Agreement
- Personal Finance
- Content
---
