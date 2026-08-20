---
api_key_in: []
api_specs:
- filename: kajabi-authentication-api-openapi.yml
  format: yaml
  label: Kajabi Authentication API
  slug: kajabi-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-authentication-api-openapi.yml
- filename: kajabi-blog-posts-api-openapi.yml
  format: yaml
  label: Kajabi Blog posts API
  slug: kajabi-blog-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-blog-posts-api-openapi.yml
- filename: kajabi-contact-notes-api-openapi.yml
  format: yaml
  label: Kajabi Contact Notes API
  slug: kajabi-contact-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-contact-notes-api-openapi.yml
- filename: kajabi-contact-tags-api-openapi.yml
  format: yaml
  label: Kajabi Contact Tags API
  slug: kajabi-contact-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-contact-tags-api-openapi.yml
- filename: kajabi-contacts-api-openapi.yml
  format: yaml
  label: Kajabi Contacts API
  slug: kajabi-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-contacts-api-openapi.yml
- filename: kajabi-courses-api-openapi.yml
  format: yaml
  label: Kajabi Courses API
  slug: kajabi-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-courses-api-openapi.yml
- filename: kajabi-custom-fields-api-openapi.yml
  format: yaml
  label: Kajabi Custom Fields API
  slug: kajabi-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-custom-fields-api-openapi.yml
- filename: kajabi-customers-api-openapi.yml
  format: yaml
  label: Kajabi Customers API
  slug: kajabi-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-customers-api-openapi.yml
- filename: kajabi-forms-api-openapi.yml
  format: yaml
  label: Kajabi Forms API
  slug: kajabi-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-forms-api-openapi.yml
- filename: kajabi-kajabi-payments-payouts-api-openapi.yml
  format: yaml
  label: Kajabi Kajabi Payments Payouts API
  slug: kajabi-kajabi-payments-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-kajabi-payments-payouts-api-openapi.yml
- filename: kajabi-landing-pages-api-openapi.yml
  format: yaml
  label: Kajabi Landing pages API
  slug: kajabi-landing-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-landing-pages-api-openapi.yml
- filename: kajabi-me-api-openapi.yml
  format: yaml
  label: Kajabi Me API
  slug: kajabi-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-me-api-openapi.yml
- filename: kajabi-offers-api-openapi.yml
  format: yaml
  label: Kajabi Offers API
  slug: kajabi-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-offers-api-openapi.yml
- filename: kajabi-orders-api-openapi.yml
  format: yaml
  label: Kajabi Orders API
  slug: kajabi-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-orders-api-openapi.yml
- filename: kajabi-podcasts-api-openapi.yml
  format: yaml
  label: Kajabi Podcasts API
  slug: kajabi-podcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-podcasts-api-openapi.yml
- filename: kajabi-products-api-openapi.yml
  format: yaml
  label: Kajabi Products API
  slug: kajabi-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-products-api-openapi.yml
- filename: kajabi-purchases-api-openapi.yml
  format: yaml
  label: Kajabi Purchases API
  slug: kajabi-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-purchases-api-openapi.yml
- filename: kajabi-sites-api-openapi.yml
  format: yaml
  label: Kajabi Sites API
  slug: kajabi-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-sites-api-openapi.yml
- filename: kajabi-transactions-api-openapi.yml
  format: yaml
  label: Kajabi Transactions API
  slug: kajabi-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-transactions-api-openapi.yml
- filename: kajabi-version-api-openapi.yml
  format: yaml
  label: Kajabi Version API
  slug: kajabi-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-version-api-openapi.yml
- filename: kajabi-webhooks-api-openapi.yml
  format: yaml
  label: Kajabi Webhooks API
  slug: kajabi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/openapi/kajabi-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kajabi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kajabi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kajabi
provider_slug: kajabi
scheme_count: 1
schemes:
- name: Bearer
  scheme: bearer
  sources:
  - openapi/kajabi-public-api-openapi.yml
  type: http
slug: kajabi-authentication
source_filename: kajabi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kajabi-public-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/kajabi-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kajabi/refs/heads/main/authentication/kajabi-authentication.yml
summary_line: http · 1 scheme
tags:
- Creator Economy
- Online Courses
- Memberships
- E-Commerce
- Digital Products
- Contacts
- Webhook
- Payments
---
