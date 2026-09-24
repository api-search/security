---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ambitioninc-openapi-generated.yml
  format: yaml
  label: Ambitioninc API
  slug: ambitioninc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambitioninc/refs/heads/main/openapi/_ae-authored/ambitioninc-openapi-generated.yml
auth_types: []
description: Token‑Based Authentication using a URL query parameter
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ambitioninc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ambitioninc declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ambitioninc
provider_slug: ambitioninc
scheme_count: 1
schemes:
- evidence: 'If you are using token-based authentication, you will need to append the following to your TV URL: ?_tva=YOUR_TOKEN_HERE'
  how_to_obtain: Request a token by emailing gethelp@ambition.com
  location: query
  name: URL token
  type: apiKey
slug: ambitioninc-authentication
source_filename: ambitioninc-authentication.yml
source_heading: Authentication Profile
source_url: https://help.ambition.com/articles/4273107736-how-can-i-display-a-tv-if-my-device-doesn-t-support-password-based-authentication
source_yaml: "generated: '2026-09-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.ambition.com/articles/4273107736-how-can-i-display-a-tv-if-my-device-doesn-t-support-password-based-authentication\nsources:\n- https://help.ambition.com/articles/4273107736-how-can-i-display-a-tv-if-my-device-doesn-t-support-password-based-authentication\n- https://help.ambition.com/articles/4369357246-how-do-i-set-up-the-coaching-quickstart-and-access-check-in-visualizations-within-domo\n- https://help.ambition.com/articles/9502903582-how-can-i-use-hidden-mode-to-test-my-competition-setup\n- https://help.ambition.com/articles/2508363429-how-do-i-set-custom-targets-or-build-ramp-time-into-scorecards\ndescription: Token‑Based Authentication using a URL query parameter\nschemes:\n- type: apiKey\n  name: URL token\n  evidence: 'If you are using token-based authentication, you will need to append the following to your TV URL: ?_tva=YOUR_TOKEN_HERE'\n  location: query\n\
  \  how_to_obtain: Request a token by emailing gethelp@ambition.com\ndocs: https://help.ambition.com/articles/4273107736-how-can-i-display-a-tv-if-my-device-doesn-t-support-password-based-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambitioninc/refs/heads/main/authentication/ambitioninc-authentication.yml
summary_line: 1 scheme
tags:
- SaaS
- Revenue Operations
- Sales Enablement
- AI
- Platform
---
