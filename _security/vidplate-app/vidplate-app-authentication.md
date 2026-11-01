---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vidplate-app-account-api-openapi.yml
  format: yaml
  label: VidPlate Account API
  slug: vidplate-app-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidplate-app/openapi/vidplate-app-account-api-openapi.yml
- filename: vidplate-app-render-nodes-api-openapi.yml
  format: yaml
  label: VidPlate Render nodes API
  slug: vidplate-app-render-nodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidplate-app/openapi/vidplate-app-render-nodes-api-openapi.yml
- filename: vidplate-app-render-presets-api-openapi.yml
  format: yaml
  label: VidPlate Render presets API
  slug: vidplate-app-render-presets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidplate-app/openapi/vidplate-app-render-presets-api-openapi.yml
- filename: vidplate-app-renders-api-openapi.yml
  format: yaml
  label: VidPlate Renders API
  slug: vidplate-app-renders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidplate-app/openapi/vidplate-app-renders-api-openapi.yml
- filename: vidplate-app-storage-destinations-api-openapi.yml
  format: yaml
  label: VidPlate Storage destinations API
  slug: vidplate-app-storage-destinations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidplate-app/openapi/vidplate-app-storage-destinations-api-openapi.yml
- filename: vidplate-app-templates-api-openapi.yml
  format: yaml
  label: VidPlate Templates API
  slug: vidplate-app-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidplate-app/openapi/vidplate-app-templates-api-openapi.yml
- filename: vidplate-app-uploads-api-openapi.yml
  format: yaml
  label: VidPlate Uploads API
  slug: vidplate-app-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidplate-app/openapi/vidplate-app-uploads-api-openapi.yml
- filename: vidplate-app-webhook-endpoints-api-openapi.yml
  format: yaml
  label: VidPlate Webhook endpoints API
  slug: vidplate-app-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vidplate-app/openapi/vidplate-app-webhook-endpoints-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Vidplate App Authentication
name_suffix: Authentication
oauth_flows: []
overview: VidPlate secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VidPlate
provider_slug: vidplate-app
scheme_count: 1
schemes:
- bearerFormat: vpk_live_...
  description: 'Workspace keys, created by workspace admins in VidPlate under Admin, then API. Scopes: templates:read (List templates, versions and their input schemas.); uploads:write (Upload images and video to use in renders.); renders:write (Create, cancel and retry renders.); renders:read (Check render status and download outputs.); webhooks:manage (Register and change webhook endpoints.); assets:read (Use A'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/vidplate-app-openapi.json
  type: http
slug: vidplate-app-authentication
source_filename: vidplate-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/vidplate-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: vpk_live_...\n  description: 'Workspace keys, created by workspace admins in VidPlate under Admin, then API.\n    Scopes: templates:read (List templates, versions and their input schemas.); uploads:write\n    (Upload images and video to use in renders.); renders:write (Create, cancel and retry renders.);\n    renders:read (Check render status and download outputs.); webhooks:manage (Register and\n    change webhook endpoints.); assets:read (Use A'\n  sources:\n  - openapi/vidplate-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/vidplate-app/authentication/vidplate-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Video
- Rendering
- API
- 3D
- Templates
---
