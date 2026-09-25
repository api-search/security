---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: American Gene Technologies International Authentication
name_suffix: Authentication
oauth_flows: []
overview: American Gene Technologies secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: American Gene Technologies
provider_slug: american-gene-technologies-international
scheme_count: 1
schemes:
- description: WordPress Application Passwords (RFC 7617 Basic over TLS). Advertised by the API index at authentication.application-passwords with the authorization endpoint https://www.americangene.com/wp-admin/authorize-application.php. Not required for any operation in this document — every operation modelled here is anonymously readable.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/american-gene-technologies-international-content-openapi.yml
  type: http
slug: american-gene-technologies-international-authentication
source_filename: american-gene-technologies-international-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: openapi/american-gene-technologies-international-content-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (RFC 7617 Basic over TLS). Advertised by the\n    API index at authentication.application-passwords with the authorization endpoint https://www.americangene.com/wp-admin/authorize-application.php.\n    Not required for any operation in this document — every operation modelled here is anonymously\n    readable.\n  sources:\n  - openapi/american-gene-technologies-international-content-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-gene-technologies-international/refs/heads/main/authentication/american-gene-technologies-international-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Biotechnology
- Life Sciences
- Gene Therapy
- Cell Therapy
- Immuno-Oncology
- HIV
- Rare Disease
- Clinical Stage
- content-api
---
