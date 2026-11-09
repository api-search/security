---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Digi Data Nl Authentication
name_suffix: Authentication
oauth_flows: []
overview: DigiData declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DigiData
provider_slug: digi-data-nl
scheme_count: 2
schemes:
- applies_to: DigiData MCP Server (https://mcp.digi-data.nl/mcp)
  bearer_methods:
  - header
  client_id_metadata_document_supported: true
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.digi-data.nl/oauth/authorize
      refreshUrl: https://mcp.digi-data.nl/oauth/token
      scopes:
        mcp:manage: ''
        mcp:read: ''
        offline_access: ''
      tokenUrl: https://mcp.digi-data.nl/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  name: mcp-oauth2
  note: Endpoints read from the published discovery documents only; none of them was called.
  pkce: S256
  registration_endpoint: https://mcp.digi-data.nl/oauth/register
  revocation_endpoint: https://mcp.digi-data.nl/oauth/revoke
  source: https://mcp.digi-data.nl/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  type: oauth2
- applies_to: DigiData OData feeds (per-customer service-root URL issued in the app)
  description_verbatim: Kies bij de verificatiemethode in Power BI voor Basic . Voer in het veld Wachtwoord je DigiData OData API-sleutel in. De gebruikersnaam mag willekeurig zijn (zoals 'apikey'), omdat DigiData de sleutel in het wachtwoordveld valideert en de gebruikersnaam negeert.
  name: odata-basic-api-key
  scheme: basic
  source: https://www.digi-data.nl/blog/odata-feed-uitleg
  type: http
slug: digi-data-nl-authentication
source_filename: digi-data-nl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://mcp.digi-data.nl/.well-known/oauth-authorization-server\n- https://mcp.digi-data.nl/.well-known/oauth-protected-resource\n- https://www.digi-data.nl/en/mcp/claude\n- https://www.digi-data.nl/blog/odata-feed-uitleg\ndocs: https://www.digi-data.nl/en/mcp/security\nsummary: Two customer-facing surfaces with separate auth. The remote MCP server (https://mcp.digi-data.nl/mcp) uses OAuth\n  2.0 authorization_code with PKCE (S256) and refresh_token, advertised via RFC 9728 protected-resource metadata and RFC 8414\n  authorization-server metadata (both fetched, HTTP 200); the user signs in to DigiData and an administrator chooses which\n  data the assistant may see. The per-customer OData feeds use HTTP Basic in Power BI with the DigiData OData API key in the\n  password field (username ignored). No OpenAPI is published; nothing here was derived from a contract.\nschemes:\n- name: mcp-oauth2\n  type: oauth2\n  applies_to:\
  \ DigiData MCP Server (https://mcp.digi-data.nl/mcp)\n  flows:\n    authorizationCode:\n      authorizationUrl: https://mcp.digi-data.nl/oauth/authorize\n      tokenUrl: https://mcp.digi-data.nl/oauth/token\n      refreshUrl: https://mcp.digi-data.nl/oauth/token\n      scopes:\n        mcp:read: ''\n        mcp:manage: ''\n        offline_access: ''\n  pkce: S256\n  grant_types:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n  - none\n  revocation_endpoint: https://mcp.digi-data.nl/oauth/revoke\n  registration_endpoint: https://mcp.digi-data.nl/oauth/register\n  client_id_metadata_document_supported: true\n  bearer_methods:\n  - header\n  source: https://mcp.digi-data.nl/.well-known/oauth-authorization-server\n  note: Endpoints read from the published discovery documents only; none of them was called.\n- name: odata-basic-api-key\n  type: http\n  scheme: basic\n  applies_to: DigiData OData feeds (per-customer service-root URL issued in the app)\n  description_verbatim:\
  \ Kies bij de verificatiemethode in Power BI voor Basic . Voer in het veld Wachtwoord je DigiData OData\n    API-sleutel in. De gebruikersnaam mag willekeurig zijn (zoals 'apikey'), omdat DigiData de sleutel in het wachtwoordveld\n    valideert en de gebruikersnaam negeert.\n  source: https://www.digi-data.nl/blog/odata-feed-uitleg\ndocs_odata: https://www.digi-data.nl/blog/odata-feed-uitleg\n"
source_yaml_url: https://artifacts.apis.io/digi-data-nl/authentication/digi-data-nl-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Business Intelligence
- Dashboards
- AI Agents
- MCP
- OData
- Power BI
- Data Integration
- Accounting
- Netherlands
---
