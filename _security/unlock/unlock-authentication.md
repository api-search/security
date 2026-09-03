---
api_key_in: []
api_specs:
- filename: unlock-site-content-api-openapi.yml
  format: yaml
  label: Unlock Site Content API
  slug: unlock-site-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-site-content-api-openapi.yml
- filename: unlock-editorial-api-openapi.yml
  format: yaml
  label: Unlock Editorial API
  slug: unlock-editorial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unlock/refs/heads/main/openapi/unlock-editorial-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
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
- Financial Services
- FinTech
- Home Equity
- Mortgage
- Real Estate
- Consumer Lending
- Home Equity Agreement
- Personal Finance
- Content
---
