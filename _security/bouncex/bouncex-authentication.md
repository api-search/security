---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bouncex-contacts-api-openapi.yml
  format: yaml
  label: Wunderkind Contacts API
  slug: bouncex-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bouncex/refs/heads/main/openapi/bouncex-contacts-api-openapi.yml
- filename: bouncex-createcontactactivities-api-openapi.yml
  format: yaml
  label: Wunderkind Createcontactactivities API
  slug: bouncex-createcontactactivities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bouncex/refs/heads/main/openapi/bouncex-createcontactactivities-api-openapi.yml
- filename: bouncex-id-resolution-api-openapi.yml
  format: yaml
  label: Wunderkind Id Resolution API
  slug: bouncex-id-resolution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bouncex/refs/heads/main/openapi/bouncex-id-resolution-api-openapi.yml
- filename: bouncex-interaction-api-openapi.yml
  format: yaml
  label: Wunderkind Interaction API
  slug: bouncex-interaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bouncex/refs/heads/main/openapi/bouncex-interaction-api-openapi.yml
- filename: bouncex-text-api-openapi.yml
  format: yaml
  label: Wunderkind Text API
  slug: bouncex-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bouncex/refs/heads/main/openapi/bouncex-text-api-openapi.yml
auth_types: []
description: Authentication methods published for Wunderkind
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bouncex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wunderkind declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Wunderkind
provider_slug: bouncex
scheme_count: 1
schemes:
- evidence: A username and password to be sent via Basic authentication
  header: Authorization
  location: header
  name: Basic
  type: http-basic
slug: bouncex-authentication
source_filename: bouncex-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.wunderkind.co/reference/authentication-security.md
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.wunderkind.co/reference/authentication-security.md\nsources:\n- https://developer.wunderkind.co/reference/authentication-security.md\n- https://developer.wunderkind.co/reference/service_apppushtokenset.md\n- https://developer.wunderkind.co/docs/msdk-getting-started.md\n- https://developer.wunderkind.co/docs/android-apppush-setup-guide.md\ndescription: Authentication methods published for Wunderkind\nschemes:\n- type: http-basic\n  name: Basic\n  evidence: A username and password to be sent via Basic authentication\n  location: header\n  header: Authorization\ndocs: https://developer.wunderkind.co/reference/authentication-security.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bouncex/refs/heads/main/authentication/bouncex-authentication.yml
summary_line: 1 scheme
tags:
- Marketing
- Artificial Intelligence
- E-Commerce
- Personalization
- Identity
---
