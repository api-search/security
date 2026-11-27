---
anonymous_access: false
api_key_in: []
auth_types: []
description: AdAce Ads API keys authenticate by sending the full key value as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AdAce Authentication
name_suffix: Authentication
oauth_flows: []
overview: AdAce declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AdAce
provider_slug: adace-website
scheme_count: 1
schemes:
- evidence: Configure the supported client to send it as an Authorization Bearer credential to the documented endpoint.
  header: Authorization
  how_to_obtain: Create a named API key in the AdAce workspace; the full key value is shown once at creation.
  location: header
  name: API Key
  type: http-bearer
slug: adace-website-authentication
source_filename: adace-website-authentication.yml
source_heading: Authentication Profile
source_url: https://ads.adace.website/en/blog/ai-clients/api-keys
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ads.adace.website/en/blog/ai-clients/api-keys\nsources:\n- https://ads.adace.website/en/blog/ai-clients/api-keys\n- https://ads.adace.website/en/blog/getting-started\n- https://ads.adace.website/ru/blog/getting-started\n- https://ads.adace.website/uk/blog/getting-started\ndescription: AdAce Ads API keys authenticate by sending the full key value as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Configure the supported client to send it as an Authorization Bearer credential to the documented endpoint.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a named API key in the AdAce workspace; the full key value is shown once at creation.\ndocs: https://ads.adace.website/en/blog/ai-clients/api-keys\n"
source_yaml_url: https://artifacts.apis.io/adace-website/authentication/adace-website-authentication.yml
summary_line: 1 scheme
tags:
- Advertising
- Lead Generation
- Marketing
- Software-as-a-Service
- Agency
---
