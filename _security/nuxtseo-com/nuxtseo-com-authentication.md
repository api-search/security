---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: nuxtseo-com-account-api-openapi.yml
  format: yaml
  label: Nuxt SEO Account API
  slug: nuxtseo-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuxtseo-com/openapi/nuxtseo-com-account-api-openapi.yml
- filename: nuxtseo-com-actions-api-openapi.yml
  format: yaml
  label: Nuxt SEO Actions API
  slug: nuxtseo-com-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuxtseo-com/openapi/nuxtseo-com-actions-api-openapi.yml
- filename: nuxtseo-com-audit-api-openapi.yml
  format: yaml
  label: Nuxt SEO Audit API
  slug: nuxtseo-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuxtseo-com/openapi/nuxtseo-com-audit-api-openapi.yml
- filename: nuxtseo-com-indexing-api-openapi.yml
  format: yaml
  label: Nuxt SEO Indexing API
  slug: nuxtseo-com-indexing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuxtseo-com/openapi/nuxtseo-com-indexing-api-openapi.yml
- filename: nuxtseo-com-pages-api-openapi.yml
  format: yaml
  label: Nuxt SEO Pages API
  slug: nuxtseo-com-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuxtseo-com/openapi/nuxtseo-com-pages-api-openapi.yml
- filename: nuxtseo-com-research-api-openapi.yml
  format: yaml
  label: Nuxt SEO Research API
  slug: nuxtseo-com-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuxtseo-com/openapi/nuxtseo-com-research-api-openapi.yml
- filename: nuxtseo-com-search-api-openapi.yml
  format: yaml
  label: Nuxt SEO Search API
  slug: nuxtseo-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuxtseo-com/openapi/nuxtseo-com-search-api-openapi.yml
- filename: nuxtseo-com-search-console-api-openapi.yml
  format: yaml
  label: Nuxt SEO Search Console API
  slug: nuxtseo-com-search-console-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuxtseo-com/openapi/nuxtseo-com-search-console-api-openapi.yml
- filename: nuxtseo-com-sitemaps-api-openapi.yml
  format: yaml
  label: Nuxt SEO Sitemaps API
  slug: nuxtseo-com-sitemaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuxtseo-com/openapi/nuxtseo-com-sitemaps-api-openapi.yml
- filename: nuxtseo-com-sites-api-openapi.yml
  format: yaml
  label: Nuxt SEO Sites API
  slug: nuxtseo-com-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuxtseo-com/openapi/nuxtseo-com-sites-api-openapi.yml
- filename: nuxtseo-com-timeline-api-openapi.yml
  format: yaml
  label: Nuxt SEO Timeline API
  slug: nuxtseo-com-timeline-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuxtseo-com/openapi/nuxtseo-com-timeline-api-openapi.yml
- filename: nuxtseo-com-web-analytics-api-openapi.yml
  format: yaml
  label: Nuxt SEO Web Analytics API
  slug: nuxtseo-com-web-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nuxtseo-com/openapi/nuxtseo-com-web-analytics-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Nuxt SEO Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuxt SEO secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nuxt SEO
provider_slug: nuxtseo-com
scheme_count: 2
schemes:
- bearerFormat: NuxtSEO API token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nuxtseo-com-openapi.yml
  type: http
- in: cookie
  name: sessionAuth
  parameter: nuxt-session
  sources:
  - openapi/nuxtseo-com-openapi.yml
  type: apiKey
slug: nuxtseo-com-authentication
source_filename: nuxtseo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nuxtseo-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: NuxtSEO API token\n  sources:\n  - openapi/nuxtseo-com-openapi.yml\n- name: sessionAuth\n  type: apiKey\n  in: cookie\n  parameter: nuxt-session\n  sources:\n  - openapi/nuxtseo-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/nuxtseo-com/authentication/nuxtseo-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- SEO
- Nuxt
- JavaScript
- Web Development
- Open Source
---
