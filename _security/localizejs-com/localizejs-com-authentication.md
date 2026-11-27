---
anonymous_access: false
api_key_in: []
api_specs:
- filename: localizejs-com-languages-api-openapi.yml
  format: yaml
  label: Localize Languages API
  slug: localizejs-com-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localizejs-com/openapi/localizejs-com-languages-api-openapi.yml
- filename: localizejs-com-projects-api-openapi.yml
  format: yaml
  label: Localize Projects API
  slug: localizejs-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localizejs-com/openapi/localizejs-com-projects-api-openapi.yml
- filename: localizejs-com-team-members-api-openapi.yml
  format: yaml
  label: Localize Team Members API
  slug: localizejs-com-team-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localizejs-com/openapi/localizejs-com-team-members-api-openapi.yml
- filename: localizejs-com-user-groups-api-openapi.yml
  format: yaml
  label: Localize User Groups API
  slug: localizejs-com-user-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/localizejs-com/openapi/localizejs-com-user-groups-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Localize Authentication
name_suffix: Authentication
oauth_flows: []
overview: Localize declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Localize
provider_slug: localizejs-com
scheme_count: 1
schemes:
- evidence: To authenticate with the API, provide your **Private Key** as the **Bearer** value in the authentication header.
  header: Authorization
  how_to_obtain: Create an API Private Key in the Localize account settings and use it as the Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: localizejs-com-authentication
source_filename: localizejs-com-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.localizejs.com/reference/api-overview.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.localizejs.com/reference/api-overview.md\nsources:\n- https://developers.localizejs.com/reference/api-overview.md\n- https://help.localizejs.com/docs/users-two-factor-authentication\n- https://help.localizejs.com/docs/two-factor-authentication\n- https://help.localizejs.com/docs/signing-up\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: To authenticate with the API, provide your **Private Key** as the **Bearer** value in the authentication header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API Private Key in the Localize account settings and use it as the Bearer token.\nnote: No other authentication schemes (apiKey, oauth2, etc.) are described on the referenced pages.\ndocs: https://developers.localizejs.com/reference/api-overview.md\n"
source_yaml_url: https://artifacts.apis.io/localizejs-com/authentication/localizejs-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Localization
- Translation
- Software-as-a-Service
---
