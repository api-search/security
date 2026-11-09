---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arcnm-io-calculations-api-openapi.yml
  format: yaml
  label: ARCNM Calculations API
  slug: arcnm-io-calculations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-calculations-api-openapi.yml
- filename: arcnm-io-calibration-api-openapi.yml
  format: yaml
  label: ARCNM Calibration API
  slug: arcnm-io-calibration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-calibration-api-openapi.yml
- filename: arcnm-io-datasets-api-openapi.yml
  format: yaml
  label: ARCNM Datasets API
  slug: arcnm-io-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-datasets-api-openapi.yml
- filename: arcnm-io-environments-api-openapi.yml
  format: yaml
  label: ARCNM Environments API
  slug: arcnm-io-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-environments-api-openapi.yml
- filename: arcnm-io-folders-api-openapi.yml
  format: yaml
  label: ARCNM Folders API
  slug: arcnm-io-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-folders-api-openapi.yml
- filename: arcnm-io-geometry-api-openapi.yml
  format: yaml
  label: ARCNM Geometry API
  slug: arcnm-io-geometry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-geometry-api-openapi.yml
- filename: arcnm-io-import-api-openapi.yml
  format: yaml
  label: ARCNM Import API
  slug: arcnm-io-import-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-import-api-openapi.yml
- filename: arcnm-io-machine-library-api-openapi.yml
  format: yaml
  label: ARCNM Machine Library API
  slug: arcnm-io-machine-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-machine-library-api-openapi.yml
- filename: arcnm-io-machines-api-openapi.yml
  format: yaml
  label: ARCNM Machines API
  slug: arcnm-io-machines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-machines-api-openapi.yml
- filename: arcnm-io-materials-api-openapi.yml
  format: yaml
  label: ARCNM Materials API
  slug: arcnm-io-materials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-materials-api-openapi.yml
- filename: arcnm-io-nesting-api-openapi.yml
  format: yaml
  label: ARCNM Nesting API
  slug: arcnm-io-nesting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-nesting-api-openapi.yml
- filename: arcnm-io-parts-api-openapi.yml
  format: yaml
  label: ARCNM Parts API
  slug: arcnm-io-parts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-parts-api-openapi.yml
- filename: arcnm-io-remnants-api-openapi.yml
  format: yaml
  label: ARCNM Remnants API
  slug: arcnm-io-remnants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-remnants-api-openapi.yml
- filename: arcnm-io-subcontractors-api-openapi.yml
  format: yaml
  label: ARCNM Subcontractors API
  slug: arcnm-io-subcontractors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-subcontractors-api-openapi.yml
- filename: arcnm-io-tools-api-openapi.yml
  format: yaml
  label: ARCNM Tools API
  slug: arcnm-io-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-tools-api-openapi.yml
- filename: arcnm-io-upload-links-api-openapi.yml
  format: yaml
  label: ARCNM Upload Links API
  slug: arcnm-io-upload-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-upload-links-api-openapi.yml
- filename: arcnm-io-uploads-api-openapi.yml
  format: yaml
  label: ARCNM Uploads API
  slug: arcnm-io-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcnm-io/openapi/arcnm-io-uploads-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Arcnm Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: ARCNM declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ARCNM
provider_slug: arcnm-io
scheme_count: 2
schemes:
- description: OAuth2 password flow for user sessions (login endpoint, disallowed to call).
  flow: password
  tokenUrl: /api/v1/sessions/login
  type: oauth2
- description: Server-to-server API key in the X-API-Key header.
  in: header
  name: X-API-Key
  type: apiKey
slug: arcnm-io-authentication
source_filename: arcnm-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://arcnm.io/docs/authentication\nschemes:\n  - type: oauth2\n    flow: password\n    tokenUrl: /api/v1/sessions/login\n    description: OAuth2 password flow for user sessions (login endpoint, disallowed to call).\n  - type: apiKey\n    in: header\n    name: X-API-Key\n    description: Server-to-server API key in the X-API-Key header.\n"
source_yaml_url: https://artifacts.apis.io/arcnm-io/authentication/arcnm-io-authentication.yml
summary_line: 2 schemes
tags:
- Manufacturing
- Costing
- CAD
- Engineering
---
