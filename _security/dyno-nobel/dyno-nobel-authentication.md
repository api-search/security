---
anonymous_access: true
api_key_in: []
api_specs:
- filename: dyno-nobel-robotslandingpage-api-openapi.yml
  format: yaml
  label: Dyno Nobel Robots Landing Page API
  slug: dyno-nobel-robotslandingpage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/openapi/dyno-nobel-robotslandingpage-api-openapi.yml
- filename: dyno-nobel-robotstext-api-openapi.yml
  format: yaml
  label: Dyno Nobel Robots Text API
  slug: dyno-nobel-robotstext-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/openapi/dyno-nobel-robotstext-api-openapi.yml
- filename: dyno-nobel-searchapi-api-openapi.yml
  format: yaml
  label: Dyno Nobel Search API
  slug: dyno-nobel-searchapi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/openapi/dyno-nobel-searchapi-api-openapi.yml
- filename: dyno-nobel-sitemanifest-api-openapi.yml
  format: yaml
  label: Dyno Nobel Site Manifest API
  slug: dyno-nobel-sitemanifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/openapi/dyno-nobel-sitemanifest-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: Dyno Nobel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dyno Nobel declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dyno Nobel
provider_slug: dyno-nobel
scheme_count: 1
schemes:
- description: No securityScheme declared in the contract; operations are unauthenticated website search endpoints.
  type: none
slug: dyno-nobel-authentication
source_filename: dyno-nobel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: derived\nsource: openapi/dyno-nobel-openapi.yml\nnote: The Swagger document (Incitech.Web, served on dev.dynonobel.com) declares no securitySchemes and no security requirement; all 16 operations are anonymous GETs used by the public website's search. There is no developer documentation describing authentication, keys or OAuth.\nschemes:\n- type: none\n  description: No securityScheme declared in the contract; operations are unauthenticated website search endpoints.\ndocs: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyno-nobel/refs/heads/main/authentication/dyno-nobel-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Explosives
- Mining
- Industrial Manufacturing
- Blasting
- Australia
---
