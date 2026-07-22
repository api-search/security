---
api_key_in:
- header
auth_types:
- oauth2
- openIdConnect
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Thingsthinking Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Thingsthinking secures its APIs with oauth2, openIdConnect, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Thingsthinking
provider_slug: thingsthinking
scheme_count: 3
schemes:
- description: Primary authentication. A domain administrator creates a client in the Administration app (Client Administration) and downloads a credentials.properties file containing client_id, client_secret and token_url. The SDK exchanges these for a bearer token against the tenant's token endpoint. server_url, client_id, client_secret and token_url can also be supplied directly.
  flow: clientCredentials
  name: OAuth2ClientCredentials
  parameters:
  - server_url
  - client_id
  - client_secret
  - token_url
  sources:
  - https://pypi.org/project/semantha-sdk/
  type: oauth2
- description: semantha recommends integrating with the customer's existing identity management system and using OpenID Connect for authentication and authorization. Other means of authentication can be made available on request.
  name: OpenIDConnect
  sources:
  - https://www.semantha.de/data-security/
  type: openIdConnect
- description: Legacy authentication (documented as "Old"). A per-domain API key grants access to a fixed number of domains; supplied to the SDK via login(server_url, key=...) or a JSON key file ({"API_Key", "server_url"}). Access is scoped to the domains bound to the key.
  in: header
  name: LegacyAPIKey
  sources:
  - https://pypi.org/project/semantha-sdk/
  - https://www.semantha.de/data-security/
  type: apiKey
slug: thingsthinking-authentication
source_filename: thingsthinking-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://pypi.org/project/semantha-sdk/\ndocs: https://www.semantha.de/data-security/\nsummary:\n  types: [oauth2, openIdConnect, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  recommended: OpenID Connect via customer identity provider\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      Primary authentication. A domain administrator creates a client in the\n      Administration app (Client Administration) and downloads a\n      credentials.properties file containing client_id, client_secret and\n      token_url. The SDK exchanges these for a bearer token against the\n      tenant's token endpoint. server_url, client_id, client_secret and\n      token_url can also be supplied directly.\n    parameters: [server_url, client_id, client_secret, token_url]\n    sources: [https://pypi.org/project/semantha-sdk/]\n  - name: OpenIDConnect\n  \
  \  type: openIdConnect\n    description: >-\n      semantha recommends integrating with the customer's existing identity\n      management system and using OpenID Connect for authentication and\n      authorization. Other means of authentication can be made available on\n      request.\n    sources: [https://www.semantha.de/data-security/]\n  - name: LegacyAPIKey\n    type: apiKey\n    in: header\n    description: >-\n      Legacy authentication (documented as \"Old\"). A per-domain API key grants\n      access to a fixed number of domains; supplied to the SDK via\n      login(server_url, key=...) or a JSON key file ({\"API_Key\", \"server_url\"}).\n      Access is scoped to the domains bound to the key.\n    sources: [https://pypi.org/project/semantha-sdk/, https://www.semantha.de/data-security/]\ntransport:\n  tls_only: true\n  note: >-\n    Neither the user interface nor the API is accessible without encryption;\n    unencrypted endpoints are not provided.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thingsthinking/refs/heads/main/authentication/thingsthinking-authentication.yml
summary_line: oauth2/openIdConnect/apiKey · 3 schemes
tags:
- Company
- Semantic AI
- Natural Language Processing
- Document Analysis
- Enterprise Search
- Contract Analysis
- Text Analytics
- Machine Learning
- Compliance
- REST API
- Germany
---
