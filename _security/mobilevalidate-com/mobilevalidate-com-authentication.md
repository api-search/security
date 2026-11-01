---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mobilevalidate-com-account-api-openapi.yml
  format: yaml
  label: mobilevalidate-com Account API
  slug: mobilevalidate-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilevalidate-com/openapi/mobilevalidate-com-account-api-openapi.yml
- filename: mobilevalidate-com-catalog-api-openapi.yml
  format: yaml
  label: mobilevalidate-com Catalog API
  slug: mobilevalidate-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilevalidate-com/openapi/mobilevalidate-com-catalog-api-openapi.yml
- filename: mobilevalidate-com-jobs-api-openapi.yml
  format: yaml
  label: mobilevalidate-com Jobs API
  slug: mobilevalidate-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilevalidate-com/openapi/mobilevalidate-com-jobs-api-openapi.yml
- filename: mobilevalidate-com-keys-api-openapi.yml
  format: yaml
  label: mobilevalidate-com Keys API
  slug: mobilevalidate-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilevalidate-com/openapi/mobilevalidate-com-keys-api-openapi.yml
- filename: mobilevalidate-com-lookup-api-openapi.yml
  format: yaml
  label: mobilevalidate-com Lookup API
  slug: mobilevalidate-com-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilevalidate-com/openapi/mobilevalidate-com-lookup-api-openapi.yml
- filename: mobilevalidate-com-system-api-openapi.yml
  format: yaml
  label: mobilevalidate-com System API
  slug: mobilevalidate-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilevalidate-com/openapi/mobilevalidate-com-system-api-openapi.yml
- filename: mobilevalidate-com-webhooks-api-openapi.yml
  format: yaml
  label: mobilevalidate-com Webhooks API
  slug: mobilevalidate-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mobilevalidate-com/openapi/mobilevalidate-com-webhooks-api-openapi.yml
auth_types: []
description: 'Every request authenticates with an API key sent as a bearer token: `Authorization: Bearer <key>`.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mobilevalidate Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: mobilevalidate-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mobilevalidate-com
provider_slug: mobilevalidate-com
scheme_count: 1
schemes:
- evidence: 'Every request authenticates with an API key sent as a bearer token: `Authorization: Bearer <key>`.'
  header: Authorization
  how_to_obtain: Create an API key in the MobileValidate developer dashboard; the key is provided once and stored as MOBILEVALIDATE_API_KEY.
  location: header
  name: Bearer
  type: http-bearer
slug: mobilevalidate-com-authentication
source_filename: mobilevalidate-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mobilevalidate.com/docs/authentication.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mobilevalidate.com/docs/authentication.md\nsources:\n- https://mobilevalidate.com/docs/authentication.md\n- https://mobilevalidate.com/docs/authentication\n- https://mobilevalidate.com/blog/silent-authentication-and-flash-call\n- https://mobilevalidate.com/docs/quickstart.md\ndescription: 'Every request authenticates with an API key sent as a bearer token: `Authorization: Bearer <key>`.'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request authenticates with an API key sent as a bearer token: `Authorization: Bearer <key>`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the MobileValidate developer dashboard; the key is provided once and stored as MOBILEVALIDATE_API_KEY.\nnote: No OAuth2, API key query, or other authentication methods are documented.\ndocs: https://mobilevalidate.com/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/mobilevalidate-com/authentication/mobilevalidate-com-authentication.yml
summary_line: 1 scheme
tags:
- Fraud Prevention
- Phone Validation
- Email Validation
- API Service
- Telecom
---
