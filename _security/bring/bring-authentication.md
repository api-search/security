---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bring-openapi-generated.yml
  format: yaml
  label: Bring API
  slug: bring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bring/openapi/_ae-authored/bring-openapi-generated.yml
auth_types: []
description: All Bring APIs require three HTTP header parameters for authentication.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Bring Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bring declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Bring
provider_slug: bring
scheme_count: 3
schemes:
- evidence: The email address of your Mybring user account.
  header: X-Mybring-API-Uid
  how_to_obtain: Use the email address of the Mybring user account.
  location: header
  name: X-Mybring-API-Uid
  type: apiKey
- evidence: The user account’s API key.
  header: X-Mybring-API-Key
  how_to_obtain: Create and manage the API key on the Mybring API page.
  location: header
  name: X-Mybring-API-Key
  type: apiKey
- evidence: The URL for the service where you are using the API.
  header: X-Bring-Client-URL
  how_to_obtain: Provide the URL of the service that will call the API.
  location: header
  name: X-Bring-Client-URL
  type: apiKey
slug: bring-authentication
source_filename: bring-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.bring.com/api
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.bring.com/api\nsources:\n- https://developer.bring.com/api\n- https://developer.bring.com/api/warehousing-api\ndescription: All Bring APIs require three HTTP header parameters for authentication.\nschemes:\n- type: apiKey\n  name: X-Mybring-API-Uid\n  evidence: The email address of your Mybring user account.\n  location: header\n  header: X-Mybring-API-Uid\n  how_to_obtain: Use the email address of the Mybring user account.\n- type: apiKey\n  name: X-Mybring-API-Key\n  evidence: The user account’s API key.\n  location: header\n  header: X-Mybring-API-Key\n  how_to_obtain: Create and manage the API key on the Mybring API page.\n- type: apiKey\n  name: X-Bring-Client-URL\n  evidence: The URL for the service where you are using the API.\n  location: header\n  header: X-Bring-Client-URL\n  how_to_obtain: Provide the URL of the service that will call the API.\ndocs:\
  \ https://developer.bring.com/api\n"
source_yaml_url: https://artifacts.apis.io/bring/authentication/bring-authentication.yml
summary_line: 3 schemes
tags:
- Logistics
- Shipping
- E‑commerce
- API
- Norway
---
