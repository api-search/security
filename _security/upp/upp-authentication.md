---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Upp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Upp. declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Upp.
provider_slug: upp
scheme_count: 1
schemes:
- evidence: Obtain an access token via OAuth to authenticate your API requests.
  flows:
  - client_credentials
  how_to_obtain: Call the token endpoint to receive an access token.
  name: OAuth
  token_url: https://svc.upp.ai/auth/oauth/token
  type: oauth2
slug: upp-authentication
source_filename: upp-authentication.yml
source_heading: Authentication Profile
source_url: https://help.upp.ai/onboarding-guide
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.upp.ai/onboarding-guide\nsources:\n- https://help.upp.ai/onboarding-guide\n- https://help.upp.ai/onboarding-upp-1\n- https://help.upp.ai/onboarding-upp-\n- https://help.upp.ai/how-to-use-upp-quick-start-guide\ndescription: Authentication\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Obtain an access token via OAuth to authenticate your API requests.\n  flows:\n  - client_credentials\n  token_url: https://svc.upp.ai/auth/oauth/token\n  how_to_obtain: Call the token endpoint to receive an access token.\ndocs: https://help.upp.ai/onboarding-guide\n"
source_yaml_url: https://artifacts.apis.io/upp/authentication/upp-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Marketing
- Advertising
- SaaS
---
