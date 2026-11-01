---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pictify-io-batch-api-openapi.yml
  format: yaml
  label: pictify-io Batch API
  slug: pictify-io-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pictify-io/openapi/pictify-io-batch-api-openapi.yml
- filename: pictify-io-bindings-api-openapi.yml
  format: yaml
  label: pictify-io Bindings API
  slug: pictify-io-bindings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pictify-io/openapi/pictify-io-bindings-api-openapi.yml
- filename: pictify-io-gifs-api-openapi.yml
  format: yaml
  label: pictify-io GIFs API
  slug: pictify-io-gifs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pictify-io/openapi/pictify-io-gifs-api-openapi.yml
- filename: pictify-io-images-api-openapi.yml
  format: yaml
  label: pictify-io Images API
  slug: pictify-io-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pictify-io/openapi/pictify-io-images-api-openapi.yml
- filename: pictify-io-pdfs-api-openapi.yml
  format: yaml
  label: pictify-io PDFs API
  slug: pictify-io-pdfs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pictify-io/openapi/pictify-io-pdfs-api-openapi.yml
- filename: pictify-io-templates-api-openapi.yml
  format: yaml
  label: pictify-io Templates API
  slug: pictify-io-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pictify-io/openapi/pictify-io-templates-api-openapi.yml
- filename: pictify-io-webhooks-api-openapi.yml
  format: yaml
  label: pictify-io Webhooks API
  slug: pictify-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pictify-io/openapi/pictify-io-webhooks-api-openapi.yml
auth_types: []
description: All API requests require authentication using an API key passed in the `Authorization` header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pictify Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: pictify-io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: pictify-io
provider_slug: pictify-io
scheme_count: 1
schemes:
- evidence: All API requests require authentication using an API key passed in the `Authorization` header.
  header: Authorization
  how_to_obtain: API keys are created on the Settings page of the dashboard (https://pictify.io/dashboard/api-token).
  location: header
  name: API Key
  type: apiKey
slug: pictify-io-authentication
source_filename: pictify-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.pictify.io/authentication.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.pictify.io/authentication.md\nsources:\n- https://docs.pictify.io/authentication.md\n- https://docs.pictify.io/security/api-keys.md\n- https://docs.pictify.io/dashboard/api-keys.md\n- https://docs.pictify.io/quickstart.md\ndescription: All API requests require authentication using an API key passed in the `Authorization` header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: All API requests require authentication using an API key passed in the `Authorization` header.\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are created on the Settings page of the dashboard (https://pictify.io/dashboard/api-token).\ndocs: https://docs.pictify.io/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/pictify-io/authentication/pictify-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Media
- API
- Templating
- Automation
---
