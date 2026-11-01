---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Unikraft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unikraft declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Unikraft
provider_slug: unikraft
scheme_count: 1
schemes:
- evidence: 'All CDP endpoints require a valid token, passed either as: Query parameter : ?token=<TOKEN>'
  location: query
  name: token
  type: apiKey
slug: unikraft-authentication
source_filename: unikraft-authentication.yml
source_heading: Authentication Profile
source_url: https://unikraft.com/docs/guides/chromium-cdp-auth
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://unikraft.com/docs/guides/chromium-cdp-auth\nsources:\n- https://unikraft.com/docs/guides/chromium-cdp-auth\n- https://unikraft.com/docs/sdks/js\n- https://unikraft.org/docs/getting-started\n- https://unikraft.org/docs/getting-started/integrations/hcp-packer\nschemes:\n- type: apiKey\n  name: token\n  evidence: 'All CDP endpoints require a valid token, passed either as: Query parameter : ?token=<TOKEN>'\n  location: query\ndocs: https://unikraft.com/docs/guides/chromium-cdp-auth\nnote: 2 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/unikraft/authentication/unikraft-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Unikernel
- OpenSource
- CloudNative
- Performance
---
