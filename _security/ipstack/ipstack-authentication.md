---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ipstack
  format: yaml
  label: ipstack REST API
  slug: ipstack-rest-api
  spec_type: Postman
  url: https://www.postman.com/apilayer/apilayer/collection/1jn3xlj/ipstack
auth_types: []
description: Two entirely different authentication models sit behind one product. The REST API uses a single static access key passed as a URL QUERY PARAMETER — the weakest of the common API key placements, since the credential lands in proxy logs, browser history and Referer headers. The MCP server in front of the same data uses a real OAuth 2.0 deployment with discovery, PKCE and dynamic client registration.
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Ipstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: IPstack declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: IPstack
provider_slug: ipstack
scheme_count: 2
schemes:
- api: ipstack REST API
  concerns:
  - Credential in the query string. It is written into access logs and CDN logs by default and is exposed in the Referer header of any resource the response loads.
  - Free tier is documented as HTTP-only in the historical plan matrix; all probes in this pass were served over HTTPS with a valid certificate.
  description: Every request appends ?access_key=YOUR_ACCESS_KEY. There is no header alternative documented and none was accepted on probe. The key is issued from the dashboard at signup and is not rotated automatically.
  evidence:
    body: '{"success":false,"error":{"code":101,"type":"missing_access_key","info":"You have not supplied an API Access Key. [Required format: access_key=YOUR_ACCESS_KEY]"}}'
    http_status: 200
    url: https://api.ipstack.com/134.201.250.155
  id: access_key
  in: query
  name: access_key
  required: true
  type: apiKey
- api: ipstack MCP Server
  authorization_endpoint: https://auth.apilayer.com/oauth2/auth
  challenge: 'WWW-Authenticate: Bearer resource_metadata="https://mcp.apilayer.com/.well-known/oauth-protected-resource"'
  code_challenge_methods:
  - S256
  description: The MCP endpoint challenges anonymous callers with a conformant RFC 9728 header and publishes full protected-resource and authorization-server metadata.
  device_authorization_endpoint: https://auth.apilayer.com/oauth2/device/auth
  evidence:
    body: '{"jsonrpc":"2.0","error":{"code":-32001,"message":"Authentication required"},"id":null}'
    http_status: 401
    url: https://mcp.apilayer.com/mcp
  grant_types:
  - authorization_code
  - implicit
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  id: apilayer_oauth
  issuer: https://auth.apilayer.com
  jwks_uri: https://auth.apilayer.com/.well-known/jwks.json
  note: The provider's own published client config uses a static bearer token (APILAYER_MCP_TOKEN) rather than the OAuth flow, so both paths appear to be accepted.
  registration_endpoint: https://auth.apilayer.com/oauth2/register
  revocation_endpoint: https://auth.apilayer.com/oauth2/revoke
  scopes:
  - openid
  - offline
  - offline_access
  - mcp:read
  - api:ipstack
  token_endpoint: https://auth.apilayer.com/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - none
  type: oauth2
slug: ipstack-authentication
source_filename: ipstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://ipstack.com/how-to-use-ipstack-api/ (HTTP 200), https://ipstack.com/llms.txt\n  (HTTP 200), live unauthenticated requests to https://api.ipstack.com/ (HTTP 200 error\n  envelopes), and the RFC 9728 / RFC 8414 discovery documents served at\n  mcp.apilayer.com and auth.apilayer.com (both HTTP 200). No OpenAPI is published, so this\n  profile was probed and read from docs rather than derived from securitySchemes.\nname: IPstack authentication profile\ndescription: >-\n  Two entirely different authentication models sit behind one product. The REST API uses a\n  single static access key passed as a URL QUERY PARAMETER — the weakest of the common\n  API key placements, since the credential lands in proxy logs, browser history and\n  Referer headers. The MCP server in front of the same data uses a real OAuth 2.0\n  deployment with discovery, PKCE and dynamic client registration.\nschemes:\n  - id: access_key\n    api:\
  \ ipstack REST API\n    type: apiKey\n    in: query\n    name: access_key\n    required: true\n    description: >-\n      Every request appends ?access_key=YOUR_ACCESS_KEY. There is no header alternative\n      documented and none was accepted on probe. The key is issued from the dashboard at\n      signup and is not rotated automatically.\n    evidence:\n      url: 'https://api.ipstack.com/134.201.250.155'\n      http_status: 200\n      body: >-\n        {\"success\":false,\"error\":{\"code\":101,\"type\":\"missing_access_key\",\"info\":\"You have\n        not supplied an API Access Key. [Required format: access_key=YOUR_ACCESS_KEY]\"}}\n    concerns:\n      - >-\n        Credential in the query string. It is written into access logs and CDN logs by\n        default and is exposed in the Referer header of any resource the response loads.\n      - >-\n        Free tier is documented as HTTP-only in the historical plan matrix; all probes in\n        this pass were served over HTTPS with\
  \ a valid certificate.\n  - id: apilayer_oauth\n    api: ipstack MCP Server\n    type: oauth2\n    description: >-\n      The MCP endpoint challenges anonymous callers with a conformant RFC 9728 header and\n      publishes full protected-resource and authorization-server metadata.\n    challenge: >-\n      WWW-Authenticate: Bearer resource_metadata=\"https://mcp.apilayer.com/.well-known/oauth-protected-resource\"\n    issuer: https://auth.apilayer.com\n    authorization_endpoint: https://auth.apilayer.com/oauth2/auth\n    token_endpoint: https://auth.apilayer.com/oauth2/token\n    registration_endpoint: https://auth.apilayer.com/oauth2/register\n    revocation_endpoint: https://auth.apilayer.com/oauth2/revoke\n    device_authorization_endpoint: https://auth.apilayer.com/oauth2/device/auth\n    jwks_uri: https://auth.apilayer.com/.well-known/jwks.json\n    grant_types:\n      - authorization_code\n      - implicit\n      - client_credentials\n      - refresh_token\n      - 'urn:ietf:params:oauth:grant-type:device_code'\n\
  \    code_challenge_methods:\n      - S256\n    token_endpoint_auth_methods:\n      - client_secret_post\n      - client_secret_basic\n      - private_key_jwt\n      - none\n    scopes:\n      - openid\n      - offline\n      - offline_access\n      - mcp:read\n      - api:ipstack\n    evidence:\n      url: https://mcp.apilayer.com/mcp\n      http_status: 401\n      body: '{\"jsonrpc\":\"2.0\",\"error\":{\"code\":-32001,\"message\":\"Authentication required\"},\"id\":null}'\n    note: >-\n      The provider's own published client config uses a static bearer token\n      (APILAYER_MCP_TOKEN) rather than the OAuth flow, so both paths appear to be accepted.\ntransport_security:\n  tls: true\n  note: >-\n    All probed hosts served valid TLS. api.ipstack.com rejects HEAD with HTTP 403 and\n    answers GET on HTTP/1.0; CORS is wide open (access-control-allow-origin: *).\ndocs:\n  - https://ipstack.com/how-to-use-ipstack-api/\n  - https://docs.apilayer.com/ipstack/docs/api-documentation\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipstack/refs/heads/main/authentication/ipstack-authentication.yml
summary_line: 2 schemes
tags:
- Geocoding
- IP Geolocation
- Location
- Threat Intelligence
- Networking
- MCP
- Public APIs
---
