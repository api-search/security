---
anonymous_access: false
api_key_in: []
api_specs:
- filename: findymail-contacts-api-openapi.yml
  format: yaml
  label: Findymail Contacts API
  slug: findymail-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-contacts-api-openapi.yml
- filename: findymail-email-finder-api-openapi.yml
  format: yaml
  label: Findymail Email Finder API
  slug: findymail-email-finder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-email-finder-api-openapi.yml
- filename: findymail-email-verifier-api-openapi.yml
  format: yaml
  label: Findymail Email Verifier API
  slug: findymail-email-verifier-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-email-verifier-api-openapi.yml
- filename: findymail-exclusion-lists-api-openapi.yml
  format: yaml
  label: Findymail Exclusion Lists API
  slug: findymail-exclusion-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-exclusion-lists-api-openapi.yml
- filename: findymail-intellimatch-api-openapi.yml
  format: yaml
  label: Findymail Intellimatch API
  slug: findymail-intellimatch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-intellimatch-api-openapi.yml
- filename: findymail-misc-api-openapi.yml
  format: yaml
  label: Findymail Misc API
  slug: findymail-misc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-misc-api-openapi.yml
- filename: findymail-phone-finder-api-openapi.yml
  format: yaml
  label: Findymail Phone Finder API
  slug: findymail-phone-finder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-phone-finder-api-openapi.yml
- filename: findymail-signals-api-openapi.yml
  format: yaml
  label: Findymail Signals API
  slug: findymail-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-signals-api-openapi.yml
- filename: findymail-technologies-api-openapi.yml
  format: yaml
  label: Findymail Technologies API
  slug: findymail-technologies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-technologies-api-openapi.yml
- filename: findymail-usage-api-openapi.yml
  format: yaml
  label: Findymail Usage API
  slug: findymail-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findymail/openapi/findymail-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Findymail Authentication
name_suffix: Authentication
oauth_flows: []
overview: Findymail secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Findymail
provider_slug: findymail
scheme_count: 1
schemes:
- description: You can retrieve your token by visiting <a href="/user/api-tokens">API page</a>.
  name: default
  scheme: bearer
  sources:
  - openapi/findymail-openapi.yml
  type: http
slug: findymail-authentication
source_filename: findymail-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/findymail-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: default\n  type: http\n  scheme: bearer\n  description: You can retrieve your token by visiting <a href=\"/user/api-tokens\">API page</a>.\n  sources:\n  - openapi/findymail-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/findymail/authentication/findymail-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Email Finder
- B2B Data
- Lead Generation
---
