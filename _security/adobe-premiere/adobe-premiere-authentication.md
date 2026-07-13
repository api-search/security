---
api_key_in: []
api_specs:
- filename: adobe-premiere-creative-cloud-libraries-openapi.yml
  format: yaml
  label: Adobe Creative Cloud Libraries API
  slug: adobe-creative-cloud-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/openapi/adobe-premiere-creative-cloud-libraries-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Premiere Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Adobe Premiere Pro secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Adobe Premiere Pro
provider_slug: adobe-premiere
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: oauth2
  sources:
  - openapi/adobe-premiere-creative-cloud-libraries-openapi.yml
  type: oauth2
slug: adobe-premiere-authentication
source_filename: adobe-premiere-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-premiere-creative-cloud-libraries-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n    scopes: 3\n  sources:\n  - openapi/adobe-premiere-creative-cloud-libraries-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-premiere/refs/heads/main/authentication/adobe-premiere-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Adobe
- Automation
- Creative Cloud
- Media
- Premiere Pro
- Video Editing
- Video Production
---
