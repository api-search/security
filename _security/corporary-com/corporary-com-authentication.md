---
anonymous_access: false
api_key_in: []
api_specs:
- filename: corporary-com-change-api-openapi.yml
  format: yaml
  label: corporary Change API
  slug: corporary-com-change-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corporary-com/openapi/corporary-com-change-api-openapi.yml
- filename: corporary-com-company-api-openapi.yml
  format: yaml
  label: corporary Company API
  slug: corporary-com-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corporary-com/openapi/corporary-com-company-api-openapi.yml
- filename: corporary-com-search-api-openapi.yml
  format: yaml
  label: corporary Search API
  slug: corporary-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corporary-com/openapi/corporary-com-search-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: corporary Authentication
name_suffix: Authentication
oauth_flows: []
overview: corporary secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: corporary
provider_slug: corporary-com
scheme_count: 2
schemes:
- description: 'Authorization: Bearer <cle>. The API is sessionless: the site cookie does not authenticate it, so no CSRF token is needed.'
  header: Authorization
  name: http
  scheme: bearer
  sources:
  - openapi/corporary-com-openapi.yml
  type: http
- description: Documented fallback for clients that cannot add the Bearer prefix; the key may also be sent bare in Authorization. Not declared in the OpenAPI.
  header: X-API-Key
  in: header
  name: X-API-Key
  sources:
  - https://corporary.com/fr/api
  type: apiKey
slug: corporary-com-authentication
source_filename: corporary-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://corporary.com/fr/api\n- https://corporary.com/docs/api\ndocs: https://corporary.com/fr/api\nsummary:\n  types:\n  - http\n  - apiKey\nschemes:\n- name: http\n  type: http\n  scheme: bearer\n  header: Authorization\n  sources:\n  - openapi/corporary-com-openapi.yml\n  description: \"Authorization: Bearer <cle>. The API is sessionless: the site cookie does not authenticate it, so no CSRF token is needed.\"\n- name: X-API-Key\n  type: apiKey\n  in: header\n  header: X-API-Key\n  sources:\n  - https://corporary.com/fr/api\n  description: Documented fallback for clients that cannot add the Bearer prefix; the key may also be sent bare in Authorization. Not declared in the OpenAPI.\nkey_management: Keys are created in the account (passwordless email sign-in link); a key is shown only once at creation.\nshared_with_mcp: true\noauth: The MCP server authenticates by key, not OAuth, per the docs.\n"
source_yaml_url: https://artifacts.apis.io/corporary-com/authentication/corporary-com-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Company Data
- Business Registry
- France
- Financial Data
- Legal Announcements
- MCP
- Open Data
---
