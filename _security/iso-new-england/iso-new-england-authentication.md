---
api_key_in: []
api_specs:
- filename: iso-new-england-web-services-openapi.yml
  format: yaml
  label: ISO New England Web Services API v1.1
  slug: iso-ne-web-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iso-new-england/refs/heads/main/openapi/iso-new-england-web-services-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Iso New England Authentication
name_suffix: Authentication
oauth_flows: []
overview: ISO New England secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ISO New England
provider_slug: iso-new-england
scheme_count: 1
schemes:
- description: HTTP Basic Authentication over SSL. Credentials come from a free, self-serve ISO Express account; ISO New England states that ISO Express account holders are automatically granted access to the public data feeds. See https://www.iso-ne.com/participate/applications-status-changes/access-software-systems
  name: basicAuth
  scheme: basic
  sources:
  - openapi/iso-new-england-web-services-openapi.yml
  type: http
slug: iso-new-england-authentication
source_filename: iso-new-england-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/iso-new-england-web-services-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication over SSL. Credentials come from a free, self-serve\n    ISO Express account; ISO New England states that ISO Express account holders are automatically\n    granted access to the public data feeds. See https://www.iso-ne.com/participate/applications-status-changes/access-software-systems\n  sources:\n  - openapi/iso-new-england-web-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iso-new-england/refs/heads/main/authentication/iso-new-england-authentication.yml
summary_line: http · 1 scheme
tags:
- Energy
- United States
- Electricity
- Energy Markets
- Grid
- Open Data
- Wholesale Markets
- Demand Response
- Renewables
- New England
---
