---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: greif-wp-json-discovery.json
  format: json
  label: Greif Website (WordPress REST)
  slug: greif-com-website-wordpress-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greif/refs/heads/main/openapi/greif-wp-json-discovery.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Greif Authentication
name_suffix: Authentication
oauth_flows: []
overview: Greif secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Greif
provider_slug: greif
scheme_count: 2
schemes:
- description: WordPress application passwords, advertised by the site's own discovery document at https://www.greif.com/wp-json/ (authentication.application-passwords.endpoints.authorization = https://www.greif.com/wp-admin/authorize-application.php). Issued only to WordPress user accounts on the Greif site; not available to third parties.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/greif-wordpress-rest-openapi.yml
  type: http
- description: WordPress logged-in cookie plus an X-WP-Nonce header — the in-browser authentication path for the site's own editors.
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/greif-wordpress-rest-openapi.yml
  type: apiKey
slug: greif-authentication
source_filename: greif-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: derived\nsource: openapi/greif-wordpress-rest-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: WordPress application passwords, advertised by the site's own discovery document\n    at https://www.greif.com/wp-json/ (authentication.application-passwords.endpoints.authorization\n    = https://www.greif.com/wp-admin/authorize-application.php). Issued only to WordPress user\n    accounts on the Greif site; not available to third parties.\n  sources:\n  - openapi/greif-wordpress-rest-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress logged-in cookie plus an X-WP-Nonce header — the in-browser authentication\n    path for the site's own editors.\n  sources:\n  - openapi/greif-wordpress-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greif/refs/heads/main/authentication/greif-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Packaging
- Industrial
- Manufacturing
- Sustainability
- Fortune 1000
---
