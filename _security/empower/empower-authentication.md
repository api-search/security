---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Empower APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Empower Authentication
name_suffix: Authentication
oauth_flows: []
overview: Empower declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Empower
provider_slug: empower
scheme_count: 2
schemes:
- evidence: The API key is used to protect the Empower API from unauthorized access. When your application makes a request to the API, the API key must be supplied as a request header named x-api-key with the value of the API key delivered.
  header: x-api-key
  how_to_obtain: Request access through the Empower developer portal; the API key is delivered via secure email after approval.
  location: header
  name: API Key
  type: apiKey
- evidence: Empower APIs use OAuth as an authorization protocol that enables applications to access information on behalf of the user. Client credentials are required per OAuth2 specification to exchange for an access token.
  flows:
  - client_credentials
  how_to_obtain: After receiving the Client ID and Client Secret via secure email, use them with Basic Auth to call the Empower authorization token endpoint (provided in the email) with grant_type=client_credentials to obtain a bearer access token.
  name: OAuth2 Client Credentials
  type: oauth2
slug: empower-authentication
source_filename: empower-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.empower.com/docs/get-started
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.empower.com/docs/get-started\nsources:\n- https://developer.empower.com/docs/get-started\ndescription: Authentication methods for Empower APIs\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The API key is used to protect the Empower API from unauthorized access. When your application makes a request to the API, the API\n    key must be supplied as a request header named x-api-key with the value of the API key delivered.\n  location: header\n  header: x-api-key\n  how_to_obtain: Request access through the Empower developer portal; the API key is delivered via secure email after approval.\n- type: oauth2\n  name: OAuth2 Client Credentials\n  evidence: Empower APIs use OAuth as an authorization protocol that enables applications to access information on behalf of the user. Client\n    credentials are required per OAuth2 specification to exchange for an access\
  \ token.\n  flows:\n  - client_credentials\n  how_to_obtain: After receiving the Client ID and Client Secret via secure email, use them with Basic Auth to call the Empower authorization\n    token endpoint (provided in the email) with grant_type=client_credentials to obtain a bearer access token.\ndocs: https://developer.empower.com/docs/get-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/empower/refs/heads/main/authentication/empower-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Investment
- Retirement
- Financial-Tools
---
