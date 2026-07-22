---
api_key_in: []
api_specs:
- filename: maintainx-openapi-original.json
  format: json
  label: MaintainX REST API v1
  slug: maintainx-rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maintainx/refs/heads/main/openapi/maintainx-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Maintainx Authentication
name_suffix: Authentication
oauth_flows: []
overview: MaintainX secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MaintainX
provider_slug: maintainx
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: '<p>Authenticate by adding the following HTTP header to your requests:</p>

    <pre>Authorization: bearer {{token}}</pre>

    <p>The <code>token</code> can be generated in your MaintainX account. Go to <a href="https://app.getmaintainx.com/settings/integrations/apiKeys">"Settings &gt; Integrations &gt; API Keys"</a> to generate a key for your user.</p>'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/maintainx-openapi-original.json
  type: http
slug: maintainx-authentication
source_filename: maintainx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/maintainx-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    <p>Authenticate by adding the following HTTP header to your requests:</p>\n    <pre>Authorization: bearer {{token}}</pre>\n    <p>The <code>token</code> can be generated in your MaintainX account. Go to <a href=\"https://app.getmaintainx.com/settings/integrations/apiKeys\">\"Settings &gt; Integrations &gt; API Keys\"</a> to generate a key for your user.</p>\n  sources:\n  - openapi/maintainx-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maintainx/refs/heads/main/authentication/maintainx-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Physical Ai
- Maintenance
- CMMS
- Asset Management
- Work Orders
- Field Service
- Manufacturing
- Preventive Maintenance
- IoT
---
