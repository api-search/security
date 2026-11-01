---
anonymous_access: false
api_key_in: []
api_specs:
- filename: html2img-com-api-openapi.json
  format: json
  label: HTML to Image API API
  slug: html-to-image-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/html2img-com/openapi/_original/html2img-com-api-openapi.json
auth_types: []
description: Authentication methods as documented
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Html2Img Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: html2img-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: html2img-com
provider_slug: html2img-com
scheme_count: 2
schemes:
- evidence: HTML to Image uses API keys to authenticate requests. Get your key from the dashboard and include it in the X-API-Key header on every request.
  header: X-API-Key
  how_to_obtain: Generate a key in the dashboard (API keys page).
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Auth: the header Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Create an API key on the API keys page (keys look like htim_...).
  location: header
  name: Authorization
  type: http-bearer
slug: html2img-com-authentication
source_filename: html2img-com-authentication.yml
source_heading: Authentication Profile
source_url: https://html2img.com/docs/authentication/
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://html2img.com/docs/authentication/\nsources:\n- https://html2img.com/docs/authentication/\n- https://html2img.com/docs/quick-start/\n- https://html2img.com/docs/getting-started/\n- https://html2img.com/docs/mcp/installation/\ndescription: Authentication methods as documented\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: HTML to Image uses API keys to authenticate requests. Get your key from the dashboard and include it in the X-API-Key header on every\n    request.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Generate a key in the dashboard (API keys page).\n- type: http-bearer\n  name: Authorization\n  evidence: 'Auth: the header Authorization: Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key on the API keys page (keys look like htim_...).\nnote: No OAuth flows or other authentication types are\
  \ documented.\ndocs: https://html2img.com/docs/authentication/\n"
source_yaml_url: https://artifacts.apis.io/html2img-com/authentication/html2img-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API
- Screenshot
- PDF
- Rendering
- HeadlessChrome
---
