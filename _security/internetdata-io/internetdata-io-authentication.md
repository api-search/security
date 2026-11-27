---
anonymous_access: false
api_key_in: []
api_specs:
- filename: internetdata-io-lookup-api-openapi.yml
  format: yaml
  label: InternetData Lookup API
  slug: internetdata-io-lookup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-lookup-api-openapi.yml
- filename: internetdata-io-entitlement-api-openapi.yml
  format: yaml
  label: InternetData Entitlement API
  slug: internetdata-io-entitlement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-entitlement-api-openapi.yml
- filename: internetdata-io-account-api-openapi.yml
  format: yaml
  label: InternetData Account API
  slug: internetdata-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-account-api-openapi.yml
- filename: internetdata-io-api-keys-api-openapi.yml
  format: yaml
  label: InternetData API keys API
  slug: internetdata-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-api-keys-api-openapi.yml
- filename: internetdata-io-authorization-api-openapi.yml
  format: yaml
  label: InternetData Authorization API
  slug: internetdata-io-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-authorization-api-openapi.yml
- filename: internetdata-io-database-api-openapi.yml
  format: yaml
  label: InternetData Database API
  slug: internetdata-io-database-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-database-api-openapi.yml
- filename: internetdata-io-database-v2-api-openapi.yml
  format: yaml
  label: InternetData Database v2 API
  slug: internetdata-io-database-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-database-v2-api-openapi.yml
- filename: internetdata-io-organization-api-openapi.yml
  format: yaml
  label: InternetData Organization API
  slug: internetdata-io-organization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/internetdata-io/openapi/internetdata-io-organization-api-openapi.yml
auth_types: []
description: Authentication schemes used by InternetData API endpoints.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: InternetData Authentication
name_suffix: Authentication
oauth_flows: []
overview: InternetData declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: InternetData
provider_slug: internetdata-io
scheme_count: 1
schemes:
- evidence: 'Any one of:


    - bearer token (scopes: apikeys.manage)'
  header: Authorization
  location: header
  name: Bearer token
  scopes:
  - apikeys.manage
  - apikeys.read
  - apikeys.reveal
  type: http-bearer
slug: internetdata-io-authentication
source_filename: internetdata-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.internetdata.io/api/api-keys/accountCreateApikey.mdx
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.internetdata.io/api/api-keys/accountCreateApikey.mdx\nsources:\n- https://docs.internetdata.io/api/api-keys/accountCreateApikey.mdx\n- https://docs.internetdata.io/api/api-keys/accountListApikeys.mdx\n- https://docs.internetdata.io/api/api-keys/accountRevealApikey.mdx\n- https://docs.internetdata.io/api/api-keys/accountRevokeApikey.mdx\ndescription: Authentication schemes used by InternetData API endpoints.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Any one of:\n\n\n    - bearer token (scopes: apikeys.manage)'\n  location: header\n  header: Authorization\n  scopes:\n  - apikeys.manage\n  - apikeys.read\n  - apikeys.reveal\ndocs: https://docs.internetdata.io/api/api-keys/accountCreateApikey.mdx\n"
source_yaml_url: https://artifacts.apis.io/internetdata-io/authentication/internetdata-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- IP Intelligence
- Data Licensing
- Geolocation
- Network Security
---
