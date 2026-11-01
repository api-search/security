---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes published on the Home Assistant documentation pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Home Assistant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Home Assistant declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Home Assistant
provider_slug: home-assistant
scheme_count: 1
schemes:
- evidence: 'Under the new authentication system you’ll see the following warning logged when the legacy API password is supplied, but not configured in Home Assistant: WARNING (MainThread) [homeassistant.components.http.auth] You need to use a bearer token to access /blah/blah from 192.0.2.4'
  header: Authorization
  how_to_obtain: Create long‑lived access tokens in User profile > Security
  location: header
  name: Long‑lived access token
  type: http-bearer
slug: home-assistant-authentication
source_filename: home-assistant-authentication.yml
source_heading: Authentication Profile
source_url: https://www.home-assistant.io/docs/authentication
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.home-assistant.io/docs/authentication\nsources:\n- https://www.home-assistant.io/docs/authentication\n- https://www.home-assistant.io/docs/authentication/providers\n- https://www.home-assistant.io/docs/authentication/multi-factor-auth\ndescription: Authentication schemes published on the Home Assistant documentation pages.\nschemes:\n- type: http-bearer\n  name: Long‑lived access token\n  evidence: 'Under the new authentication system you’ll see the following warning logged when the legacy API password is supplied, but not configured\n    in Home Assistant: WARNING (MainThread) [homeassistant.components.http.auth] You need to use a bearer token to access /blah/blah from 192.0.2.4'\n  location: header\n  header: Authorization\n  how_to_obtain: Create long‑lived access tokens in User profile > Security\ndocs: https://www.home-assistant.io/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/home-assistant/authentication/home-assistant-authentication.yml
summary_line: 1 scheme
tags:
- Home Automation
- Open Source
- IoT
- Community
- Nonprofit
---
