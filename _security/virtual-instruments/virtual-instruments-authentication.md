---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Virtual Instruments Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Virtana (Virtual Instruments) secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Virtana (Virtual Instruments)
provider_slug: virtual-instruments
scheme_count: 2
schemes:
- credential_source: client_id / client_secret are minted via the "Generate OAuth Credentials" workflow in the Virtana Platform.
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2 client credentials (Virtana Platform / Global View)
  parameters:
  - client_id
  - client_secret
  request_example: curl --location 'https://app.cloud.virtana.com/authorization/oauth/token' --form 'grant_type="client_credentials"' --form 'client_id="<client_id>"' --form 'client_secret="<client_secret>"'
  response_fields:
  - access_token
  - refresh_token
  - expires_in
  - scope
  - token_type
  token_type: Bearer
  token_url: https://app.cloud.virtana.com/authorization/oauth/token
  type: oauth2
- header: 'Authorization: Bearer <your-io-api-token>'
  name: IO API bearer token (Infrastructure Observability)
  notes: IO Swagger UI (releases 7.1.0+) exposes an Authorize button to input the API token, and the downloadable OpenAPI YAML for use in tools like Postman.
  scheme: bearer
  token_source: Generated from the IO UI (User Name > API Documentation / API Token Management). Only users with the IO-admin privilege can generate a token for a specific timeframe; the token grants API access to anyone holding it while valid.
  type: http
slug: virtual-instruments-authentication
source_filename: virtual-instruments-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.virtana.com/en/virtana-platform/about-oauth-credentials/get-bearer-token.html\ndocs:\n  - https://docs.virtana.com/en/virtana-platform/about-oauth-credentials.html\n  - https://docs.virtana.com/en/virtana-platform/about-oauth-credentials/generate-oauth-credentials.html\n  - https://docs.virtana.com/en/virtana-platform/about-oauth-credentials/get-bearer-token.html\n  - https://docs.virtana.com/en/infrastructure-observability/io-user-guide/public-api/getting-started-with-the-public-api.html\n  - https://docs.virtana.com/en/infrastructure-observability/io-administrator-guide/administering-your-io-portal/api-token-management.html\nsummary:\n  types: [oauth2, http]\n  oauth2_flows: [clientCredentials]\n  http_schemes: [bearer]\n  token_delivery: Authorization header, prefixed with \"Bearer\"\nschemes:\n  - name: OAuth2 client credentials (Virtana Platform / Global View)\n    type: oauth2\n    flow: clientCredentials\n\
  \    token_url: https://app.cloud.virtana.com/authorization/oauth/token\n    grant_type: client_credentials\n    parameters: [client_id, client_secret]\n    request_example: >-\n      curl --location 'https://app.cloud.virtana.com/authorization/oauth/token'\n      --form 'grant_type=\"client_credentials\"' --form 'client_id=\"<client_id>\"'\n      --form 'client_secret=\"<client_secret>\"'\n    response_fields: [access_token, refresh_token, expires_in, scope, token_type]\n    token_type: Bearer\n    credential_source: >-\n      client_id / client_secret are minted via the \"Generate OAuth Credentials\"\n      workflow in the Virtana Platform.\n  - name: IO API bearer token (Infrastructure Observability)\n    type: http\n    scheme: bearer\n    header: 'Authorization: Bearer <your-io-api-token>'\n    token_source: >-\n      Generated from the IO UI (User Name > API Documentation / API Token\n      Management). Only users with the IO-admin privilege can generate a token\n      for a specific\
  \ timeframe; the token grants API access to anyone holding it\n      while valid.\n    notes: >-\n      IO Swagger UI (releases 7.1.0+) exposes an Authorize button to input the\n      API token, and the downloadable OpenAPI YAML for use in tools like Postman.\nnotes:\n  - No public OpenAPI/Swagger document is available off-appliance; the IO OpenAPI YAML is downloadable only from an authenticated IO appliance instance at https://<IPADDRESS>/api/sdk/p/index.html.\n  - Global View and IO MCP endpoints reuse the same OAuth token / bearer token respectively (see mcp/virtual-instruments-mcp.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtual-instruments/refs/heads/main/authentication/virtual-instruments-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Infrastructure
- Observability
- Monitoring
- Storage
- Cloud Cost Management
- AIOps
- Performance
- Alerts
- MCP
---
