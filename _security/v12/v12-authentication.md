---
anonymous_access: false
api_key_in: []
api_specs:
- filename: v12-documents-api-openapi.yml
  format: yaml
  label: V12 Documents API
  slug: v12-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-documents-api-openapi.yml
- filename: v12-findings-api-openapi.yml
  format: yaml
  label: V12 Findings API
  slug: v12-findings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-findings-api-openapi.yml
- filename: v12-me-api-openapi.yml
  format: yaml
  label: V12 Me API
  slug: v12-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-me-api-openapi.yml
- filename: v12-members-api-openapi.yml
  format: yaml
  label: V12 Members API
  slug: v12-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-members-api-openapi.yml
- filename: v12-repositories-api-openapi.yml
  format: yaml
  label: V12 Repositories API
  slug: v12-repositories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-repositories-api-openapi.yml
- filename: v12-runs-api-openapi.yml
  format: yaml
  label: V12 Runs API
  slug: v12-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-runs-api-openapi.yml
- filename: v12-steers-api-openapi.yml
  format: yaml
  label: V12 Steers API
  slug: v12-steers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/v12/openapi/v12-steers-api-openapi.yml
auth_types: []
description: Authentication for V12 API uses Bearer tokens sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: V12 Authentication
name_suffix: Authentication
oauth_flows: []
overview: V12 declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: V12
provider_slug: v12
scheme_count: 2
schemes:
- evidence: Send the token only in the Authorization header, as Bearer <token> . The API ignores a token in a cookie or the query string.
  header: Authorization
  how_to_obtain: Create it in Settings → Developer ; see Create an API key . Token prefix is v12p_ .
  location: header
  name: API key
  type: http-bearer
- evidence: Send the token only in the Authorization header, as Bearer <token> . The API ignores a token in a cookie or the query string.
  header: Authorization
  how_to_obtain: Sign in through the browser and approve the consent page. Token prefix is v12a_ .
  location: header
  name: OAuth access token
  type: http-bearer
slug: v12-authentication
source_filename: v12-authentication.yml
source_heading: Authentication Profile
source_url: https://v12.sh/docs/public-api/authentication
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://v12.sh/docs/public-api/authentication\nsources:\n- https://v12.sh/docs/public-api/authentication\n- https://v12.sh/docs/quickstart\n- https://v12.sh/docs/public-api/quickstart\ndescription: Authentication for V12 API uses Bearer tokens sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: Send the token only in the Authorization header, as Bearer <token> . The API ignores a token in a cookie or the query string.\n  location: header\n  header: Authorization\n  how_to_obtain: Create it in Settings → Developer ; see Create an API key . Token prefix is v12p_ .\n- type: http-bearer\n  name: OAuth access token\n  evidence: Send the token only in the Authorization header, as Bearer <token> . The API ignores a token in a cookie or the query string.\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in through the browser\
  \ and approve the consent page. Token prefix is v12a_ .\ndocs: https://v12.sh/docs/public-api/authentication\n"
source_yaml_url: https://artifacts.apis.io/v12/authentication/v12-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Security
- DevOps
- Automation
- Code Analysis
---
