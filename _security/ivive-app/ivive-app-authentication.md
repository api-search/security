---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ivive-app-auth-api-openapi.yml
  format: yaml
  label: ivive.app Auth API
  slug: ivive-app-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-auth-api-openapi.yml
- filename: ivive-app-correction-equations-api-openapi.yml
  format: yaml
  label: ivive.app Correction Equations API
  slug: ivive-app-correction-equations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-correction-equations-api-openapi.yml
- filename: ivive-app-health-api-openapi.yml
  format: yaml
  label: ivive.app Health API
  slug: ivive-app-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-health-api-openapi.yml
- filename: ivive-app-ivivc-api-openapi.yml
  format: yaml
  label: ivive.app Ivivc API
  slug: ivive-app-ivivc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-ivivc-api-openapi.yml
- filename: ivive-app-ivive-api-openapi.yml
  format: yaml
  label: ivive.app Ivive API
  slug: ivive-app-ivive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-ivive-api-openapi.yml
- filename: ivive-app-library-api-openapi.yml
  format: yaml
  label: ivive.app Library API
  slug: ivive-app-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-library-api-openapi.yml
- filename: ivive-app-molecule-api-openapi.yml
  format: yaml
  label: ivive.app Molecule API
  slug: ivive-app-molecule-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-molecule-api-openapi.yml
- filename: ivive-app-pk-api-openapi.yml
  format: yaml
  label: ivive.app Pk API
  slug: ivive-app-pk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-pk-api-openapi.yml
- filename: ivive-app-prediction-api-openapi.yml
  format: yaml
  label: ivive.app Prediction API
  slug: ivive-app-prediction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-prediction-api-openapi.yml
- filename: ivive-app-reference-compounds-api-openapi.yml
  format: yaml
  label: ivive.app Reference Compounds API
  slug: ivive-app-reference-compounds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-reference-compounds-api-openapi.yml
- filename: ivive-app-scaling-api-openapi.yml
  format: yaml
  label: ivive.app Scaling API
  slug: ivive-app-scaling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ivive-app/openapi/ivive-app-scaling-api-openapi.yml
auth_types: []
description: Authentication for ivive.app API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ivive.app Authentication
name_suffix: Authentication
oauth_flows: []
overview: ivive.app declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ivive.app
provider_slug: ivive-app
scheme_count: 1
schemes:
- evidence: 'Returns a Bearer JWT token. Token lifetime: 24 hours. Include in subsequent requests as: Authorization: Bearer'
  header: Authorization
  how_to_obtain: POST /api/auth/login with email and password to receive an access_token
  location: header
  name: Bearer JWT
  type: http-bearer
slug: ivive-app-authentication
source_filename: ivive-app-authentication.yml
source_heading: Authentication Profile
source_url: https://api.ivive.app/docs#/auth
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.ivive.app/docs#/auth\nsources:\n- https://api.ivive.app/docs#/auth\n- https://api.ivive.app/docs#/auth/register_api_auth_register_post\n- https://api.ivive.app/docs#/auth/login_api_auth_login_post\n- https://api.ivive.app/docs#/auth/me_api_auth_me_get\ndescription: Authentication for ivive.app API\nschemes:\n- type: http-bearer\n  name: Bearer JWT\n  evidence: 'Returns a Bearer JWT token. Token lifetime: 24 hours. Include in subsequent requests as: Authorization: Bearer'\n  location: header\n  header: Authorization\n  how_to_obtain: POST /api/auth/login with email and password to receive an access_token\ndocs: https://api.ivive.app/docs#/auth\n"
source_yaml_url: https://artifacts.apis.io/ivive-app/authentication/ivive-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- IVIVE
- Drug Discovery
- HepaticClearance
- Open Source
---
