---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Orionis Biosciences Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orionis Biosciences secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Orionis Biosciences
provider_slug: orionis-biosciences
scheme_count: 2
schemes:
- description: WordPress Application Passwords (RFC 7617 Basic). The site advertises the authorization endpoint https://orionisbio.com/wp-admin/authorize-application.php in its /wp-json/ root document. Write access only; not issued to the public.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/orionis-biosciences-content-openapi.yml
  type: http
- description: WordPress cookie authentication with an X-WP-Nonce header (first-party browser context only).
  in: header
  name: cookieNonce
  parameter: X-WP-Nonce
  sources:
  - openapi/orionis-biosciences-content-openapi.yml
  type: apiKey
slug: orionis-biosciences-authentication
source_filename: orionis-biosciences-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/orionis-biosciences-content-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (RFC 7617 Basic). The site advertises the authorization\n    endpoint https://orionisbio.com/wp-admin/authorize-application.php in its /wp-json/ root\n    document. Write access only; not issued to the public.\n  sources:\n  - openapi/orionis-biosciences-content-openapi.yml\n- name: cookieNonce\n  type: apiKey\n  in: header\n  parameter: X-WP-Nonce\n  description: WordPress cookie authentication with an X-WP-Nonce header (first-party browser\n    context only).\n  sources:\n  - openapi/orionis-biosciences-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orionis-biosciences/refs/heads/main/authentication/orionis-biosciences-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Drug Discovery
- Pharmaceuticals
- Oncology
- Immunotherapy
- Protein Engineering
- Molecular Glues
- Computational Biology
- Machine Learning
- Clinical Trials
- Content
---
