---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Hivelocity API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hivelocity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hivelocity declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hivelocity
provider_slug: hivelocity
scheme_count: 1
schemes:
- evidence: Each request to the API requires an HTTP Request called `X-API-KEY` with the value being your API Key.
  header: X-API-KEY
  how_to_obtain: You must generate an API key in your *myVelocity Control Panel*.
  location: header
  name: apiKey
  type: apiKey
slug: hivelocity-authentication
source_filename: hivelocity-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.hivelocity.net/docs/api-keys.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.hivelocity.net/docs/api-keys.md\nsources:\n- https://developers.hivelocity.net/docs/api-keys.md\n- https://developers.hivelocity.net/reference/get_saml_service_provider_config_resource.md\n- https://developers.hivelocity.net/reference/delete_saml_service_provider_config_resource.md\n- https://developers.hivelocity.net/reference/post_saml_service_provider_config_resource.md\ndescription: Authentication schemes for Hivelocity API\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: Each request to the API requires an HTTP Request called `X-API-KEY` with the value being your API Key.\n  location: header\n  header: X-API-KEY\n  how_to_obtain: You must generate an API key in your *myVelocity Control Panel*.\ndocs: https://developers.hivelocity.net/docs/api-keys.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hivelocity/refs/heads/main/authentication/hivelocity-authentication.yml
summary_line: 1 scheme
tags:
- Cloud
- Hosting
- BareMetal
- VPS
- Colocation
- Infrastructure
---
