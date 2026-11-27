---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ideogram-subpackage-datasets-api-openapi.yml
  format: yaml
  label: Ideogram Subpackage Datasets API
  slug: ideogram-subpackage-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-subpackage-datasets-api-openapi.yml
- filename: ideogram-subpackage-generate-api-openapi.yml
  format: yaml
  label: Ideogram Subpackage Generate API
  slug: ideogram-subpackage-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-subpackage-generate-api-openapi.yml
- filename: ideogram-subpackage-models-api-openapi.yml
  format: yaml
  label: Ideogram Subpackage Models API
  slug: ideogram-subpackage-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-subpackage-models-api-openapi.yml
- filename: ideogram-subpackage-vision-api-openapi.yml
  format: yaml
  label: Ideogram Subpackage Vision API
  slug: ideogram-subpackage-vision-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-subpackage-vision-api-openapi.yml
- filename: ideogram-account-api-openapi.yml
  format: yaml
  label: Ideogram Account API
  slug: ideogram-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-account-api-openapi.yml
- filename: ideogram-auto-model-api-openapi.yml
  format: yaml
  label: Ideogram Auto Model API
  slug: ideogram-auto-model-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-auto-model-api-openapi.yml
- filename: ideogram-design-api-openapi.yml
  format: yaml
  label: Ideogram Design API
  slug: ideogram-design-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-design-api-openapi.yml
- filename: ideogram-edit-workflow-api-openapi.yml
  format: yaml
  label: Ideogram Edit Workflow API
  slug: ideogram-edit-workflow-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-edit-workflow-api-openapi.yml
- filename: ideogram-generations-api-openapi.yml
  format: yaml
  label: Ideogram Generations API
  slug: ideogram-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-generations-api-openapi.yml
- filename: ideogram-image-describe-api-openapi.yml
  format: yaml
  label: Ideogram Image Describe API
  slug: ideogram-image-describe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-image-describe-api-openapi.yml
- filename: ideogram-images-generate-api-openapi.yml
  format: yaml
  label: Ideogram Images Generate API
  slug: ideogram-images-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-images-generate-api-openapi.yml
- filename: ideogram-images-inpaint-api-openapi.yml
  format: yaml
  label: Ideogram Images Inpaint API
  slug: ideogram-images-inpaint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-images-inpaint-api-openapi.yml
- filename: ideogram-images-precise-edit-api-openapi.yml
  format: yaml
  label: Ideogram Images Precise Edit API
  slug: ideogram-images-precise-edit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-images-precise-edit-api-openapi.yml
- filename: ideogram-images-remix-api-openapi.yml
  format: yaml
  label: Ideogram Images Remix API
  slug: ideogram-images-remix-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-images-remix-api-openapi.yml
- filename: ideogram-images-upscale-api-openapi.yml
  format: yaml
  label: Ideogram Images Upscale API
  slug: ideogram-images-upscale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-images-upscale-api-openapi.yml
- filename: ideogram-object-removal-api-openapi.yml
  format: yaml
  label: Ideogram Object Removal API
  slug: ideogram-object-removal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-object-removal-api-openapi.yml
- filename: ideogram-reframe-api-openapi.yml
  format: yaml
  label: Ideogram Reframe API
  slug: ideogram-reframe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-reframe-api-openapi.yml
- filename: ideogram-tool-api-openapi.yml
  format: yaml
  label: Ideogram Tool API
  slug: ideogram-tool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-tool-api-openapi.yml
- filename: ideogram-tools-api-openapi.yml
  format: yaml
  label: Ideogram Tools API
  slug: ideogram-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-tools-api-openapi.yml
- filename: ideogram-video-edit-api-openapi.yml
  format: yaml
  label: Ideogram Video Edit API
  slug: ideogram-video-edit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-video-edit-api-openapi.yml
- filename: ideogram-video-generate-api-openapi.yml
  format: yaml
  label: Ideogram Video Generate API
  slug: ideogram-video-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ideogram/openapi/ideogram-video-generate-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Ideogram Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ideogram secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ideogram
provider_slug: ideogram
scheme_count: 1
schemes:
- description: API key for access control. Use in the header with the name \"Api-Key\"
  in: header
  name: ApiKeyAuth
  parameter: Api-Key
  sources:
  - openapi/ideogram-openapi.yml
  type: apiKey
slug: ideogram-authentication
source_filename: ideogram-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ideogram-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: API key for access control. Use in the header with the name \\\"Api-Key\\\"\n  sources:\n  - openapi/ideogram-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/ideogram/authentication/ideogram-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Image Generation
- Text
- Realistic
- Editing
---
