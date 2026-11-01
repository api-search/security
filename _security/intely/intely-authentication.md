---
anonymous_access: false
api_key_in: []
api_specs:
- filename: intely-apps-api-openapi.yml
  format: yaml
  label: Intely Apps API
  slug: intely-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intely/openapi/intely-apps-api-openapi.yml
- filename: intely-connect-api-openapi.yml
  format: yaml
  label: Intely Connect API
  slug: intely-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intely/openapi/intely-connect-api-openapi.yml
- filename: intely-data-processor-api-openapi.yml
  format: yaml
  label: Intely Data Processor API
  slug: intely-data-processor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intely/openapi/intely-data-processor-api-openapi.yml
- filename: intely-forms-api-openapi.yml
  format: yaml
  label: Intely Forms API
  slug: intely-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intely/openapi/intely-forms-api-openapi.yml
- filename: intely-identity-management-api-openapi.yml
  format: yaml
  label: Intely Identity Management API
  slug: intely-identity-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intely/openapi/intely-identity-management-api-openapi.yml
- filename: intely-rosetta-api-openapi.yml
  format: yaml
  label: Intely Rosetta API
  slug: intely-rosetta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intely/openapi/intely-rosetta-api-openapi.yml
- filename: intely-storage-api-openapi.yml
  format: yaml
  label: Intely Storage API
  slug: intely-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intely/openapi/intely-storage-api-openapi.yml
- filename: intely-webhooks-api-openapi.yml
  format: yaml
  label: Intely Webhooks API
  slug: intely-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intely/openapi/intely-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for Intely API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Intely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intely declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Intely
provider_slug: intely
scheme_count: 2
schemes:
- evidence: The API key
  location: query
  name: api_key
  type: apiKey
- evidence: This endpoint uses basic auth. The username is the user's username and the password is the personal access token.
  header: Authorization
  how_to_obtain: Generate a Personal Access Token in your Intely account (My Profile → Create New Token) and use it as the password with your platform username for basic authentication to retrieve a user token.
  location: header
  name: personal_token
  type: http-basic
slug: intely-authentication
source_filename: intely-authentication.yml
source_heading: Authentication Profile
source_url: https://documentation.intely.io/reference/get_forms-api-key-validate.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://documentation.intely.io/reference/get_forms-api-key-validate.md\nsources:\n- https://documentation.intely.io/reference/get_forms-api-key-validate.md\n- https://documentation.intely.io/reference/get_forms-api-key-validate\n- https://documentation.intely.io/docs/authentication\n- https://documentation.intely.io/reference/post_noauth-user-login-token.md\ndescription: Authentication schemes for Intely API\nschemes:\n- type: apiKey\n  name: api_key\n  evidence: The API key\n  location: query\n- type: http-basic\n  name: personal_token\n  evidence: This endpoint uses basic auth. The username is the user's username and the password is the personal access token.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a Personal Access Token in your Intely account (My Profile → Create New Token) and use it as the password with your\n    platform username for basic\
  \ authentication to retrieve a user token.\ndocs: https://documentation.intely.io/reference/get_forms-api-key-validate.md\n"
source_yaml_url: https://artifacts.apis.io/intely/authentication/intely-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Low-Code
- Automation
- API Platform
- Enterprise
---
