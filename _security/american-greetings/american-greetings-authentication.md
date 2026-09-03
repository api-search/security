---
api_key_in: []
api_specs:
- filename: american-greetings-corporate-wordpress-rest-openapi.yml
  format: yaml
  label: American Greetings Corporate WordPress REST API
  slug: american-greetings-corporate-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/american-greetings/refs/heads/main/openapi/american-greetings-corporate-wordpress-rest-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: American Greetings Authentication
name_suffix: Authentication
oauth_flows: []
overview: American Greetings secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: American Greetings
provider_slug: american-greetings
scheme_count: 1
schemes:
- description: WordPress application passwords. Authorization endpoint advertised by the provider at https://corporate.americangreetings.com/wp-admin/authorize-application.php
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/american-greetings-corporate-wordpress-rest-openapi.yml
  type: http
slug: american-greetings-authentication
source_filename: american-greetings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: derived\nsource: openapi/american-greetings-corporate-wordpress-rest-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress application passwords. Authorization endpoint advertised by the provider\n    at https://corporate.americangreetings.com/wp-admin/authorize-application.php\n  sources:\n  - openapi/american-greetings-corporate-wordpress-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-greetings/refs/heads/main/authentication/american-greetings-authentication.yml
summary_line: http · 1 scheme
tags:
- Greeting Cards
- Gift Wrap
- Celebration
- Consumer Products
- Retail
- Stationery
- Party Supplies
- Digital Greetings
- Content API
- WordPress REST API
---
