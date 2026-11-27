---
anonymous_access: false
api_key_in: []
api_specs:
- filename: merofoundry-com-forms-api-openapi.yml
  format: yaml
  label: MeroFoundry Forms API
  slug: merofoundry-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merofoundry-com/openapi/merofoundry-com-forms-api-openapi.yml
- filename: merofoundry-com-pages-api-openapi.yml
  format: yaml
  label: MeroFoundry Pages API
  slug: merofoundry-com-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merofoundry-com/openapi/merofoundry-com-pages-api-openapi.yml
- filename: merofoundry-com-public-api-openapi.yml
  format: yaml
  label: MeroFoundry Public API
  slug: merofoundry-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merofoundry-com/openapi/merofoundry-com-public-api-openapi.yml
- filename: merofoundry-com-push-devices-api-openapi.yml
  format: yaml
  label: MeroFoundry push devices API
  slug: merofoundry-com-push-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merofoundry-com/openapi/merofoundry-com-push-devices-api-openapi.yml
- filename: merofoundry-com-records-api-openapi.yml
  format: yaml
  label: MeroFoundry Records API
  slug: merofoundry-com-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merofoundry-com/openapi/merofoundry-com-records-api-openapi.yml
- filename: merofoundry-com-stats-api-openapi.yml
  format: yaml
  label: MeroFoundry Stats API
  slug: merofoundry-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/merofoundry-com/openapi/merofoundry-com-stats-api-openapi.yml
auth_types: []
description: Authentication via API key
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MeroFoundry Authentication
name_suffix: Authentication
oauth_flows: []
overview: MeroFoundry declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MeroFoundry
provider_slug: merofoundry-com
scheme_count: 1
schemes:
- evidence: 'Header: X-API-Key: mf_<marker>_<token> # on every request'
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
slug: merofoundry-com-authentication
source_filename: merofoundry-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.merofoundry.app/authoring-interactive-pages-api-key
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.merofoundry.app/authoring-interactive-pages-api-key\nsources:\n- https://docs.merofoundry.app/authoring-interactive-pages-api-key\n- https://docs.merofoundry.app/recipes/authentication-basics\n- https://docs.merofoundry.app/recipes/secure-authentication\n- https://docs.merofoundry.app/recipes/tool-delete-push-credentials\ndescription: Authentication via API key\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Header: X-API-Key: mf_<marker>_<token> # on every request'\n  location: header\n  header: X-API-Key\ndocs: https://docs.merofoundry.app/authoring-interactive-pages-api-key\n"
source_yaml_url: https://artifacts.apis.io/merofoundry-com/authentication/merofoundry-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Platform
- Application Development
- Low-Code
- Privacy
---
