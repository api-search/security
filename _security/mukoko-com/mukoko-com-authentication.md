---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mukoko-com-news-api-openapi.yml
  format: yaml
  label: Mukoko News API
  slug: mukoko-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mukoko-com/openapi/mukoko-com-news-api-openapi.yml
- filename: mukoko-com-service-api-openapi.yml
  format: yaml
  label: Mukoko Service API
  slug: mukoko-com-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mukoko-com/openapi/mukoko-com-service-api-openapi.yml
- filename: mukoko-com-weather-api-openapi.yml
  format: yaml
  label: Mukoko Weather API
  slug: mukoko-com-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mukoko-com/openapi/mukoko-com-weather-api-openapi.yml
auth_types: []
description: All API endpoints are authenticated using Bearer tokens and picked up from the specification file.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mukoko Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mukoko declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mukoko
provider_slug: mukoko-com
scheme_count: 1
schemes:
- evidence: All API endpoints are authenticated using Bearer tokens and picked up from the specification file.
  header: Authorization
  location: header
  name: bearerAuth
  type: http-bearer
slug: mukoko-com-authentication
source_filename: mukoko-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.mukoko.com/api-reference/introduction#authentication
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.mukoko.com/api-reference/introduction#authentication\nsources:\n- https://docs.mukoko.com/api-reference/introduction#authentication\n- https://docs.mukoko.com/quickstart.md\n- https://docs.mukoko.com/ai-tools/cursor.md\n- https://docs.mukoko.com/ai-tools/claude-code.md\ndescription: All API endpoints are authenticated using Bearer tokens and picked up from the specification file.\nschemes:\n- type: http-bearer\n  name: bearerAuth\n  evidence: All API endpoints are authenticated using Bearer tokens and picked up from the specification file.\n  location: header\n  header: Authorization\ndocs: https://docs.mukoko.com/api-reference/introduction#authentication\n"
source_yaml_url: https://artifacts.apis.io/mukoko-com/authentication/mukoko-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Super App
- Africa
- Event
- Weather
- News
---
