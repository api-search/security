---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Formspree Authentication
name_suffix: Authentication
oauth_flows: []
overview: Formspree secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Formspree
provider_slug: formspree
scheme_count: 1
schemes:
- description: 'Basic auth with empty username and the form API key as password

    (e.g. `curl -u :API_KEY https://formspree.io/api/0/forms/{hashid}/submissions`).'
  name: apiKeyBasic
  scheme: basic
  sources:
  - openapi/formspree-openapi.yml
  type: http
slug: formspree-authentication
source_filename: formspree-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/formspree-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKeyBasic\n  type: http\n  scheme: basic\n  description: |-\n    Basic auth with empty username and the form API key as password\n    (e.g. `curl -u :API_KEY https://formspree.io/api/0/forms/{hashid}/submissions`).\n  sources:\n  - openapi/formspree-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formspree/refs/heads/main/authentication/formspree-authentication.yml
summary_line: http · 1 scheme
tags:
- Forms
- Backend
- Static Sites
- Email
- Webhooks
- JAMstack
- CLI
---
