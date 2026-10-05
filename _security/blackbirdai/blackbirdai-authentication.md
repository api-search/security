---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Blackbird.AI API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Blackbirdai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blackbird.AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Blackbird.AI
provider_slug: blackbirdai
scheme_count: 2
schemes:
- evidence: Your client credentials (Client ID and Client Secret) for the Client Credentials flow.
  flows:
  - client_credentials
  how_to_obtain: Client ID and Client Secret from your Blackbird AI account
  name: OAuth2 Client Credentials
  token_url: https://api.blackbird.ai/auth/oauth2/token
  type: oauth2
- evidence: (Not reccommended in a production integration) Alternatively for trying out the API, your Compass Application username + password.
  flows:
  - password
  how_to_obtain: Compass Application username and password
  name: OAuth2 Password Grant
  token_url: https://api.blackbird.ai/compass/token
  type: oauth2
slug: blackbirdai-authentication
source_filename: blackbirdai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.blackbird.ai/token.md
source_yaml: "generated: '2026-09-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.blackbird.ai/token.md\nsources:\n- https://docs.blackbird.ai/token.md\n- https://docs.blackbird.ai/quickstart.md\ndescription: Authentication methods for Blackbird.AI API\nschemes:\n- type: oauth2\n  name: OAuth2 Client Credentials\n  evidence: Your client credentials (Client ID and Client Secret) for the Client Credentials flow.\n  flows:\n  - client_credentials\n  token_url: https://api.blackbird.ai/auth/oauth2/token\n  how_to_obtain: Client ID and Client Secret from your Blackbird AI account\n- type: oauth2\n  name: OAuth2 Password Grant\n  evidence: (Not reccommended in a production integration) Alternatively for trying out the API, your Compass Application username + password.\n  flows:\n  - password\n  token_url: https://api.blackbird.ai/compass/token\n  how_to_obtain: Compass Application username and password\ndocs: https://docs.blackbird.ai/token.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackbirdai/refs/heads/main/authentication/blackbirdai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Risk Intelligence
- Data Analytics
- Enterprise
---
