---
anonymous_access: false
api_key_in: []
api_specs:
- filename: groniz-com-openapi-generated.yml
  format: yaml
  label: Groniz API
  slug: groniz-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/groniz-com/openapi/_ae-authored/groniz-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Groniz
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Groniz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Groniz declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Groniz
provider_slug: groniz-com
scheme_count: 3
schemes:
- evidence: 'All endpoints require an API key passed in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Get your API key from Groniz Settings page.
  location: header
  name: ApiKeyAuth
  type: apiKey
- authorize_url: https://groniz.com/console/connectors/oauth/authorize?client_id={CLIENT_ID}&response_type=code&state={STATE}
  evidence: Groniz supports OAuth2 Authorization Code flow, allowing you to build third‑party applications that act on behalf of Groniz users.
  flows:
  - authorization_code
  how_to_obtain: Register an OAuth app in the Groniz dashboard under API Keys → Apps to receive a Client ID and Client Secret.
  name: OAuth2 Authorization Code
  token_url: https://{BACKEND_URL}/oauth/token
  type: oauth2
- evidence: 'Authenticate using the device flow — no client ID or secret needed:'
  flows:
  - device
  how_to_obtain: Run `groniz auth login` which displays a one‑time code and opens a browser for authorization.
  name: OAuth2 Device Flow (CLI)
  type: oauth2
slug: groniz-com-authentication
source_filename: groniz-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.groniz.com/cli/authentication.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.groniz.com/cli/authentication.md\nsources:\n- https://docs.groniz.com/cli/authentication.md\n- https://docs.groniz.com/troubleshooting/oauth-connect.md\n- https://docs.groniz.com/public-api/integrations/connect.md\n- https://docs.groniz.com/public-api/oauth.md\ndescription: Authentication methods for Groniz\nschemes:\n- type: apiKey\n  name: ApiKeyAuth\n  evidence: 'All endpoints require an API key passed in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Get your API key from Groniz Settings page.\n- type: oauth2\n  name: OAuth2 Authorization Code\n  evidence: Groniz supports OAuth2 Authorization Code flow, allowing you to build third‑party applications that act on behalf of Groniz users.\n  flows:\n  - authorization_code\n  token_url: https://{BACKEND_URL}/oauth/token\n  authorize_url: https://groniz.com/console/connectors/oauth/authorize?client_id={CLIENT_ID}&response_type=code&state={STATE}\n\
  \  how_to_obtain: Register an OAuth app in the Groniz dashboard under API Keys → Apps to receive a Client ID and Client Secret.\n- type: oauth2\n  name: OAuth2 Device Flow (CLI)\n  evidence: 'Authenticate using the device flow — no client ID or secret needed:'\n  flows:\n  - device\n  how_to_obtain: Run `groniz auth login` which displays a one‑time code and opens a browser for authorization.\ndocs: https://docs.groniz.com/cli/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/groniz-com/authentication/groniz-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Social Media
- Artificial Intelligence
- Automation
- Marketing
---
