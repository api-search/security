---
anonymous_access: false
api_key_in: []
api_specs:
- filename: databox-openapi-generated.yml
  format: yaml
  label: Databox API
  slug: databox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databox/openapi/_ae-authored/databox-openapi-generated.yml
auth_types: []
description: Authentication schemes for Databox API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Databox Authentication
name_suffix: Authentication
oauth_flows: []
overview: Databox declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Databox
provider_slug: databox
scheme_count: 1
schemes:
- evidence: To access the API, you must authenticate requests using an API key.
  header: x-api-key
  how_to_obtain: Create a new key on the Profile page (Account Management > Profile) in the Password & Security section.
  location: header
  name: API key
  type: apiKey
slug: databox-authentication
source_filename: databox-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.databox.com/docs/v1/api/authentication.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.databox.com/docs/v1/api/authentication.md\nsources:\n- https://developers.databox.com/docs/v1/api/authentication.md\n- https://developers.databox.com/docs/api/authentication.md\n- https://developers.databox.com/docs/api/authentication\n- https://developers.databox.com/docs/api/api.databox.com/auth/auth_validateapikey\ndescription: Authentication schemes for Databox API\nschemes:\n- type: apiKey\n  name: API key\n  evidence: To access the API, you must authenticate requests using an API key.\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a new key on the Profile page (Account Management > Profile) in the Password & Security section.\nnote: Support for OAuth 2.0 is coming soon; no OAuth flows are documented.\ndocs: https://developers.databox.com/docs/v1/api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/databox/authentication/databox-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Analytics
- AI
- Data Integration
- Business Intelligence
---
