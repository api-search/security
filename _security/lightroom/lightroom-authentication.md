---
api_key_in:
- header
api_specs:
- filename: lightroom-album-assets-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Album Assets API
  slug: lightroom-album-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-album-assets-api-openapi.yml
- filename: lightroom-albums-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Albums API
  slug: lightroom-albums-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-albums-api-openapi.yml
- filename: lightroom-assets-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Assets API
  slug: lightroom-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-assets-api-openapi.yml
- filename: lightroom-auto-straighten-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Auto Straighten API
  slug: lightroom-auto-straighten-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-auto-straighten-api-openapi.yml
- filename: lightroom-auto-tone-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Auto Tone API
  slug: lightroom-auto-tone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-auto-tone-api-openapi.yml
- filename: lightroom-catalog-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Catalog API
  slug: lightroom-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-catalog-api-openapi.yml
- filename: lightroom-edit-image-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Edit Image API
  slug: lightroom-edit-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-edit-image-api-openapi.yml
- filename: lightroom-health-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Health API
  slug: lightroom-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-health-api-openapi.yml
- filename: lightroom-master-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Master API
  slug: lightroom-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-master-api-openapi.yml
- filename: lightroom-presets-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Presets API
  slug: lightroom-presets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-presets-api-openapi.yml
- filename: lightroom-renditions-api-openapi.yml
  format: yaml
  label: Adobe Lightroom Renditions API
  slug: lightroom-renditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-renditions-api-openapi.yml
- filename: lightroom-xmp-api-openapi.yml
  format: yaml
  label: Adobe Lightroom XMP API
  slug: lightroom-xmp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/openapi/lightroom-xmp-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Lightroom Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Adobe Lightroom secures its APIs with apiKey and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Adobe Lightroom
provider_slug: lightroom
scheme_count: 3
schemes:
- flows:
  - authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: oauth2
  sources:
  - openapi/lightroom-albums-openapi.yml
  - openapi/lightroom-assets-openapi.yml
  - openapi/lightroom-catalog-openapi.yml
  - openapi/lightroom-services-openapi.yml
  type: oauth2
- in: header
  name: apiKey
  parameter: X-Api-Key
  sources:
  - openapi/lightroom-albums-openapi.yml
  - openapi/lightroom-assets-openapi.yml
  - openapi/lightroom-catalog-openapi.yml
  - openapi/lightroom-firefly-services-openapi.yml
  - openapi/lightroom-services-openapi.yml
  type: apiKey
- description: OAuth 2.0 via Adobe IMS for Firefly Services
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3
  name: oauth2
  sources:
  - openapi/lightroom-firefly-services-openapi.yml
  type: oauth2
slug: lightroom-authentication
source_filename: lightroom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lightroom-albums-openapi.yml, openapi/lightroom-assets-openapi.yml, openapi/lightroom-catalog-openapi.yml,\n  openapi/lightroom-firefly-services-openapi.yml, openapi/lightroom-services-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ims-na1.adobelogin.com/ims/authorize/v2\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n    scopes: 1\n  sources:\n  - openapi/lightroom-albums-openapi.yml\n  - openapi/lightroom-assets-openapi.yml\n  - openapi/lightroom-catalog-openapi.yml\n  - openapi/lightroom-services-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/lightroom-albums-openapi.yml\n  - openapi/lightroom-assets-openapi.yml\n  - openapi/lightroom-catalog-openapi.yml\n\
  \  - openapi/lightroom-firefly-services-openapi.yml\n  - openapi/lightroom-services-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://ims-na1.adobelogin.com/ims/token/v3\n    scopes: 2\n  description: OAuth 2.0 via Adobe IMS for Firefly Services\n  sources:\n  - openapi/lightroom-firefly-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightroom/refs/heads/main/authentication/lightroom-authentication.yml
summary_line: apiKey/oauth2 · 3 schemes
tags:
- Cloud Storage
- Image Editing
- Metadata
- Photo Management
- Photography
---
