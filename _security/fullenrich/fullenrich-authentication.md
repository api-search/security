---
api_key_in: []
api_specs:
- filename: fullenrich-openapi.yml
  format: yaml
  label: FullEnrich Contact Enrichment API
  slug: fullenrich-contact-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-openapi.yml
- filename: fullenrich-openapi.yml
  format: yaml
  label: FullEnrich Enrichment Results API
  slug: fullenrich-enrichment-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-openapi.yml
- filename: fullenrich-openapi.yml
  format: yaml
  label: FullEnrich Reverse Email Lookup API
  slug: fullenrich-reverse-email-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-openapi.yml
- filename: fullenrich-openapi.yml
  format: yaml
  label: FullEnrich Account Credits API
  slug: fullenrich-account-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/openapi/fullenrich-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fullenrich Authentication
name_suffix: Authentication
oauth_flows: []
overview: FullEnrich secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FullEnrich
provider_slug: fullenrich
scheme_count: 1
schemes:
- description: 'Pass your API key from the FullEnrich dashboard as a Bearer token in the Authorization header: `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fullenrich-openapi.yml
  type: http
slug: fullenrich-authentication
source_filename: fullenrich-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fullenrich-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Pass your API key from the FullEnrich dashboard as a Bearer token in the Authorization\n    header: `Authorization: Bearer [example key]`.'\n  sources:\n  - openapi/fullenrich-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fullenrich/refs/heads/main/authentication/fullenrich-authentication.yml
summary_line: http · 1 scheme
tags:
- B2B Data
- Contact Enrichment
- Email Finder
- Phone Finder
- Waterfall Enrichment
- Sales Intelligence
---
