---
anonymous_access: false
api_key_in: []
api_specs:
- filename: diamondpaintingconverter-com-openapi-generated.yml
  format: yaml
  label: Diamond Painting Converter API
  slug: diamondpaintingconverter-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/diamondpaintingconverter-com/openapi/_ae-authored/diamondpaintingconverter-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Diamondpaintingconverter Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Diamond Painting Converter declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Diamond Painting Converter
provider_slug: diamondpaintingconverter-com
scheme_count: 2
schemes:
- format: 'Authorization: Bearer dp_live_xxxxxxxxxxxxxxxx'
  header: Authorization
  key_prefix: dp_live_
  name: bearer
  provisioning: Contact the PicDP team to request an API key. The key is displayed once when created — store it securely.
  scheme: bearer
  type: http
  use: server integrations
- in: html-attribute
  key_prefix: dp_embed_
  name: embed-key
  note: Never include a dp_live_ server key in browser code.
  type: apiKey
  use: browser script-tag widget; domain-bound to the exact store origin, selected in the dashboard
slug: diamondpaintingconverter-com-authentication
source_filename: diamondpaintingconverter-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://diamondpaintingconverter.com/api/docs\ndocs: https://diamondpaintingconverter.com/api/docs#authentication\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Authorization: Bearer dp_live_xxxxxxxxxxxxxxxx'\n  key_prefix: dp_live_\n  use: server integrations\n  provisioning: Contact the PicDP team to request an API key. The key is displayed once when created — store it securely.\n- name: embed-key\n  type: apiKey\n  in: html-attribute\n  key_prefix: dp_embed_\n  use: browser script-tag widget; domain-bound to the exact store origin, selected in the dashboard\n  note: Never include a dp_live_ server key in browser code.\nnotes:\n- Authentication errors (401) may use the default DRF error format in the response body.\n"
source_yaml_url: https://artifacts.apis.io/diamondpaintingconverter-com/authentication/diamondpaintingconverter-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Diamond Painting
- Image Processing
- E-Commerce
- Previews
- Webshop Integrations
- Arts and Crafts
---
