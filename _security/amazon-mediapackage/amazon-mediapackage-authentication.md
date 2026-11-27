---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-mediapackage-channels-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Channels API
  slug: amazon-mediapackage-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediapackage/openapi/amazon-mediapackage-channels-api-openapi.yml
- filename: amazon-mediapackage-harvest-jobs-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Harvest Jobs API
  slug: amazon-mediapackage-harvest-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediapackage/openapi/amazon-mediapackage-harvest-jobs-api-openapi.yml
- filename: amazon-mediapackage-origin-endpoints-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Origin Endpoints API
  slug: amazon-mediapackage-origin-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediapackage/openapi/amazon-mediapackage-origin-endpoints-api-openapi.yml
- filename: amazon-mediapackage-tags-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Tags API
  slug: amazon-mediapackage-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediapackage/openapi/amazon-mediapackage-tags-api-openapi.yml
- filename: amazon-mediapackage-assets-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Mediapackage Assets API
  slug: amazon-mediapackage-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediapackage/openapi/amazon-mediapackage-assets-api-openapi.yml
- filename: amazon-mediapackage-channelgroup-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Mediapackage Channelgroup API
  slug: amazon-mediapackage-channelgroup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediapackage/openapi/amazon-mediapackage-channelgroup-api-openapi.yml
- filename: amazon-mediapackage-operations-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Mediapackage Operations API
  slug: amazon-mediapackage-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediapackage/openapi/amazon-mediapackage-operations-api-openapi.yml
- filename: amazon-mediapackage-packaging-configurations-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Mediapackage Packaging Configurations API
  slug: amazon-mediapackage-packaging-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediapackage/openapi/amazon-mediapackage-packaging-configurations-api-openapi.yml
- filename: amazon-mediapackage-packaging-groups-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Mediapackage Packaging Groups API
  slug: amazon-mediapackage-packaging-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediapackage/openapi/amazon-mediapackage-packaging-groups-api-openapi.yml
- filename: amazon-mediapackage-policy-api-openapi.yml
  format: yaml
  label: Amazon MediaPackage Mediapackage Policy API
  slug: amazon-mediapackage-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediapackage/openapi/amazon-mediapackage-policy-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon MediaPackage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon MediaPackage secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon MediaPackage
provider_slug: amazon-mediapackage
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-mediapackage-assets-api-openapi.yml
  - openapi/amazon-mediapackage-channelgroup-api-openapi.yml
  - openapi/amazon-mediapackage-channels-api-openapi.yml
  - openapi/amazon-mediapackage-harvest-jobs-api-openapi.yml
  - openapi/amazon-mediapackage-operations-api-openapi.yml
  - openapi/amazon-mediapackage-origin-endpoints-api-openapi.yml
  - openapi/amazon-mediapackage-packaging-configurations-api-openapi.yml
  - openapi/amazon-mediapackage-packaging-groups-api-openapi.yml
  - openapi/amazon-mediapackage-policy-api-openapi.yml
  - openapi/amazon-mediapackage-tags-api-openapi.yml
  type: apiKey
slug: amazon-mediapackage-authentication
source_filename: amazon-mediapackage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-mediapackage-assets-api-openapi.yml, openapi/amazon-mediapackage-channelgroup-api-openapi.yml,\n  openapi/amazon-mediapackage-channels-api-openapi.yml, openapi/amazon-mediapackage-harvest-jobs-api-openapi.yml,\n  openapi/amazon-mediapackage-operations-api-openapi.yml, openapi/amazon-mediapackage-origin-endpoints-api-openapi.yml,\n  openapi/amazon-mediapackage-packaging-configurations-api-openapi.yml, openapi/amazon-mediapackage-packaging-groups-api-openapi.yml,\n  openapi/amazon-mediapackage-policy-api-openapi.yml, openapi/amazon-mediapackage-tags-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary\n    credentials).\
  \ Not a bearer token.\n  sources:\n  - openapi/amazon-mediapackage-assets-api-openapi.yml\n  - openapi/amazon-mediapackage-channelgroup-api-openapi.yml\n  - openapi/amazon-mediapackage-channels-api-openapi.yml\n  - openapi/amazon-mediapackage-harvest-jobs-api-openapi.yml\n  - openapi/amazon-mediapackage-operations-api-openapi.yml\n  - openapi/amazon-mediapackage-origin-endpoints-api-openapi.yml\n  - openapi/amazon-mediapackage-packaging-configurations-api-openapi.yml\n  - openapi/amazon-mediapackage-packaging-groups-api-openapi.yml\n  - openapi/amazon-mediapackage-policy-api-openapi.yml\n  - openapi/amazon-mediapackage-tags-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-mediapackage/authentication/amazon-mediapackage-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Broadcasting
- Media Processing
- Media
---
