---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fabric-so-openapi-generated.yml
  format: yaml
  label: Fabric API
  slug: fabric-so-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabric-so/openapi/_ae-authored/fabric-so-openapi-generated.yml
auth_types: []
description: Authentication schemes for Fabric API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fabric So Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fabric declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Fabric
provider_slug: fabric-so
scheme_count: 2
schemes:
- evidence: 'To authenticate your requests, you need to pass the API key with the header: X-Api-Key: <API_KEY>.'
  header: X-Api-Key
  location: header
  name: Personal API key
  type: apiKey
- evidence: 'Once you complete the authentication flow and acquire an access token, pass it with the header Authorization: Bearer <ACCESS_TOKEN>.'
  header: Authorization
  location: header
  name: OAuth 2.0
  type: oauth2
slug: fabric-so-authentication
source_filename: fabric-so-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.fabric.so/developer-guide/getting-started
source_yaml: "generated: '2026-10-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.fabric.so/developer-guide/getting-started\nsources:\n- https://developers.fabric.so/developer-guide/getting-started\ndescription: Authentication schemes for Fabric API\nschemes:\n- type: apiKey\n  name: Personal API key\n  evidence: 'To authenticate your requests, you need to pass the API key with the header: X-Api-Key: <API_KEY>.'\n  location: header\n  header: X-Api-Key\n- type: oauth2\n  name: OAuth 2.0\n  evidence: 'Once you complete the authentication flow and acquire an access token, pass it with the header Authorization: Bearer <ACCESS_TOKEN>.'\n  location: header\n  header: Authorization\ndocs: https://developers.fabric.so/developer-guide/getting-started\n"
source_yaml_url: https://artifacts.apis.io/fabric-so/authentication/fabric-so-authentication.yml
summary_line: 2 schemes
tags:
- AI Workspace
- File Storage
- Integrations
---
