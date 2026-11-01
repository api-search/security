---
anonymous_access: false
api_key_in: []
api_specs:
- filename: creduse-openapi-generated.yml
  format: yaml
  label: Creduse API
  slug: creduse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creduse/openapi/_ae-authored/creduse-openapi-generated.yml
auth_types: []
description: Authentication schemes for Creduse API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Creduse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Creduse declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Creduse
provider_slug: creduse
scheme_count: 1
schemes:
- evidence: 'All API requests should include your API key in an Authorization HTTP header as follows: http Authorization : Bearer $YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Generate an API key by navigating to the API Key section of your account.
  location: header
  name: API Key
  type: apiKey
slug: creduse-authentication
source_filename: creduse-authentication.yml
source_heading: Authentication Profile
source_url: https://doc.creduse.com/api-reference/getting-started
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://doc.creduse.com/api-reference/getting-started\nsources:\n- https://doc.creduse.com/api-reference/getting-started\ndescription: Authentication schemes for Creduse API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'All API requests should include your API key in an Authorization HTTP header as follows: http Authorization : Bearer $YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key by navigating to the API Key section of your account.\ndocs: https://doc.creduse.com/api-reference/getting-started\n"
source_yaml_url: https://artifacts.apis.io/creduse/authentication/creduse-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
