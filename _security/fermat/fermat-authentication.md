---
api_key_in: []
api_specs:
- filename: fermat-pixel-asyncapi.yml
  format: yaml
  label: FERMAT Pixel v2
  slug: fermat-pixel-v2
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fermat/refs/heads/main/asyncapi/fermat-pixel-asyncapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Fermat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fermat declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Fermat
provider_slug: fermat
scheme_count: 3
schemes:
- applies_to: https://mcp.fermatcommerce.com/mcp/fermat-mcp
  bearer_methods_supported:
  - header
  challenge: '401 with WWW-Authenticate: Bearer resource_metadata="https://mcp.fermatcommerce.com/.well-known/oauth-protected-resource/mcp/fermat-mcp"'
  description: OAuth 2.1 authorization-code + PKCE against the FERMAT Platform MCP server. Users sign in with existing FERMAT platform credentials; the provider names Auth0 as the identity provider.
  flows:
    authorizationCode:
      authorizationUrl: https://mcp.fermatcommerce.com/mcp/fermat-mcp/authorize
      authorization_response_iss_parameter_supported: true
      code_challenge_methods:
      - S256
      dynamic_client_registration: true
      grant_types:
      - authorization_code
      - refresh_token
      issuer: https://mcp.fermatcommerce.com/mcp/fermat-mcp
      registrationUrl: https://mcp.fermatcommerce.com/mcp/fermat-mcp/register
      response_types:
      - code
      revocationUrl: https://mcp.fermatcommerce.com/mcp/fermat-mcp/revoke
      scopes: {}
      tokenUrl: https://mcp.fermatcommerce.com/mcp/fermat-mcp/token
      token_endpoint_auth_methods:
      - client_secret_basic
      - client_secret_post
      - none
  id: fermat-mcp-oauth
  type: oauth2
- applies_to: https://e.clairedefermat.com, https://sr.clairedefermat.com
  description: Browser pixel identification. The FERMAT Pixel v2 is initialized with a per-brand Pixel ID issued by a FERMAT representative; it is a public client-side identifier, not a secret credential.
  id: fermat-pixel-id
  in: body
  name: config.id
  source: https://help.fermatcommerce.com/en/articles/14280269-fermat-pixel-v2-installation-guide-direct-script-google-tag-manager
  type: apiKey
- applies_to: https://mcp.fermatcommerce.com/mcp/fermat-mcp
  description: The MCP install snippets require six caller-supplied credential headers (Mcp-Elmo-Api-Key, Mcp-Reddit-Client-Id/Secret/Username/Password, Mcp-Search-Api-Url), indicating the server proxies third-party systems using the caller's own credentials. Values are operator-supplied and unpublished.
  id: mcp-pass-through-headers
  in: header
  type: apiKey
slug: fermat-authentication
source_filename: fermat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.fermatcommerce.com/.well-known/oauth-authorization-server/mcp/fermat-mcp + https://help.fermatcommerce.com/en/articles/14431099-fermat-mcp-connect-your-commerce-data-to-ai-tools\nnote: FERMAT publishes no OpenAPI, so this profile is not derived from securitySchemes. It is read from\n  the live RFC 8414 authorization-server metadata the MCP host serves anonymously, plus the provider help\n  article.\nschemes:\n- id: fermat-mcp-oauth\n  type: oauth2\n  description: OAuth 2.1 authorization-code + PKCE against the FERMAT Platform MCP server. Users sign\n    in with existing FERMAT platform credentials; the provider names Auth0 as the identity provider.\n  applies_to: https://mcp.fermatcommerce.com/mcp/fermat-mcp\n  flows:\n    authorizationCode:\n      issuer: https://mcp.fermatcommerce.com/mcp/fermat-mcp\n      authorizationUrl: https://mcp.fermatcommerce.com/mcp/fermat-mcp/authorize\n      tokenUrl: https://mcp.fermatcommerce.com/mcp/fermat-mcp/token\n\
  \      registrationUrl: https://mcp.fermatcommerce.com/mcp/fermat-mcp/register\n      revocationUrl: https://mcp.fermatcommerce.com/mcp/fermat-mcp/revoke\n      grant_types:\n      - authorization_code\n      - refresh_token\n      response_types:\n      - code\n      code_challenge_methods:\n      - S256\n      token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - none\n      dynamic_client_registration: true\n      authorization_response_iss_parameter_supported: true\n      scopes: {}\n  bearer_methods_supported:\n  - header\n  challenge: '401 with WWW-Authenticate: Bearer resource_metadata=\"https://mcp.fermatcommerce.com/.well-known/oauth-protected-resource/mcp/fermat-mcp\"'\n- id: fermat-pixel-id\n  type: apiKey\n  in: body\n  name: config.id\n  description: Browser pixel identification. The FERMAT Pixel v2 is initialized with a per-brand Pixel\n    ID issued by a FERMAT representative; it is a public client-side identifier, not a secret credential.\n\
  \  applies_to: https://e.clairedefermat.com, https://sr.clairedefermat.com\n  source: https://help.fermatcommerce.com/en/articles/14280269-fermat-pixel-v2-installation-guide-direct-script-google-tag-manager\n- id: mcp-pass-through-headers\n  type: apiKey\n  in: header\n  description: The MCP install snippets require six caller-supplied credential headers (Mcp-Elmo-Api-Key,\n    Mcp-Reddit-Client-Id/Secret/Username/Password, Mcp-Search-Api-Url), indicating the server proxies\n    third-party systems using the caller's own credentials. Values are operator-supplied and unpublished.\n  applies_to: https://mcp.fermatcommerce.com/mcp/fermat-mcp\nonboarding:\n  self_serve: false\n  note: No public sign-up for API/MCP access. The provider FAQ states an active FERMAT account is required\n    and directs prospects to their FERMAT account team; Pixel IDs are issued by a FERMAT representative.\nscopes_published: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fermat/refs/heads/main/authentication/fermat-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Commerce
- E-Commerce
- Personalization
- Analytics
- Conversion Rate Optimization
- Artificial Intelligence
- Merchandising
- MCP
- Agentic Commerce
- Session Replay
- Experimentation
- Attribution
---
