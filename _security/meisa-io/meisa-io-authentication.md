---
anonymous_access: false
api_key_in: []
auth_types: []
description: Meisa authenticates requests using an API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Meisa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Meisa declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Meisa
provider_slug: meisa-io
scheme_count: 1
schemes:
- evidence: Every request is authenticated with an API key sent in the X-API-Key header.
  header: X-API-Key
  how_to_obtain: Create an API key in the Meisa dashboard under Settings → API Keys and copy the key.
  location: header
  name: X-API-Key
  type: apiKey
slug: meisa-io-authentication
source_filename: meisa-io-authentication.yml
source_heading: Authentication Profile
source_url: https://meisa.io/docs/authentication
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://meisa.io/docs/authentication\nsources:\n- https://meisa.io/docs/authentication\n- https://help.meisa.io/articles/create-an-api-key\n- https://meisa.io/docs/quickstart\n- https://help.meisa.io/collections/getting-started\ndescription: Meisa authenticates requests using an API key.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Every request is authenticated with an API key sent in the X-API-Key header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API key in the Meisa dashboard under Settings → API Keys and copy the key.\ndocs: https://meisa.io/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/meisa-io/authentication/meisa-io-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Software-as-a-Service
- Onboarding
- Lifecycle
- Newsletters
---
