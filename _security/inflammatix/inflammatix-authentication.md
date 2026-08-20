---
api_key_in: []
api_specs:
- filename: inflammatix-content-openapi.yml
  format: yaml
  label: Inflammatix Site Content API
  slug: site-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-content-openapi.yml
- filename: inflammatix-support-content-openapi.yml
  format: yaml
  label: Inflammatix Support and Training Content API
  slug: support-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-support-content-openapi.yml
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
