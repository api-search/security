---
api_key_in:
- header
api_specs:
- filename: zoho-campaigns-email-api-collection.json
  format: json
  label: Zoho Campaigns Email API
  slug: zoho-campaigns-email-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/zoho-campaigns/refs/heads/main/postman/zoho-campaigns-email-api-collection.json
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Zoho Campaigns Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zoho Campaigns secures its APIs with oauth2 and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zoho Campaigns
provider_slug: zoho-campaigns
scheme_count: 3
schemes:
- access_token_lifetime: 1 hour
  api: Zoho Campaigns API v1.1
  authorizationUrl: https://accounts.zoho.com/oauth/v2/auth
  flow: authorizationCode
  header: 'Authorization: Zoho-oauthtoken <access_token>'
  introspectionUrl: https://accounts.zoho.com/oauth/v2/introspect
  name: ZohoOAuth
  prerequisites:
  - A client registered in Zoho Accounts (client id + client secret)
  - Requested scopes granted by the Zoho Campaigns account owner
  refresh: A refresh token is issued alongside the access token; use it against the Zoho Accounts token endpoint to mint a new access token when the current one expires.
  revocationUrl: https://accounts.zoho.com/oauth/v2/token/revoke
  scopes_reference: scopes/zoho-campaigns-scopes.yml
  source: https://www.zoho.com/campaigns/help/developers/access-token.html
  tokenUrl: https://accounts.zoho.com/oauth/v2/token
  type: oauth2
- api: Zoho Campaigns Email API v2
  generation: Zoho Campaigns console -> API Keys -> Create API Key; name the key and select the scope.
  in: header
  key_limit: Maximum of 20 API keys per user
  name: ZohoAPIKey
  parameter_name: Authorization
  scope: ZohoCampaigns.emailapi.ALL
  source: https://www.zoho.com/campaigns/help/emailapi/authentication.html
  type: apiKey
  value_format: Zoho-zapikey <api_key>
- api: Zoho Campaigns Email API v1
  flow: authorizationCode
  name: ZohoOAuthEmailAPI
  note: The Email API v1 surface in the provider's own Postman collection is grouped as "v1 - OAuth" and authenticates with the same Zoho Accounts OAuth 2.0 tokens; v2 replaced it with the Zoho-zapikey API key above.
  source: postman/zoho-campaigns-email-api-collection.json
  type: oauth2
slug: zoho-campaigns-authentication
source_filename: zoho-campaigns-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.zoho.com/campaigns/help/developers/access-token.html\ndocs:\n  - https://www.zoho.com/campaigns/help/developers/access-token.html\n  - https://www.zoho.com/campaigns/help/emailapi/authentication.html\nnote: >-\n  Derived by hand from the provider's published authentication documentation.\n  Zoho Campaigns publishes no OpenAPI, so there are no securitySchemes to derive\n  from; every value below is quoted from the two developer-guide pages named in\n  docs[], plus the OIDC discovery document served by the authorization server at\n  accounts.zoho.com.\nsummary:\n  types:\n    - oauth2\n    - apiKey\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorizationCode\n  authorization_server: https://accounts.zoho.com\nschemes:\n  - name: ZohoOAuth\n    api: Zoho Campaigns API v1.1\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n\
  \    revocationUrl: https://accounts.zoho.com/oauth/v2/token/revoke\n    introspectionUrl: https://accounts.zoho.com/oauth/v2/introspect\n    header: 'Authorization: Zoho-oauthtoken <access_token>'\n    access_token_lifetime: 1 hour\n    refresh: >-\n      A refresh token is issued alongside the access token; use it against the\n      Zoho Accounts token endpoint to mint a new access token when the current\n      one expires.\n    prerequisites:\n      - A client registered in Zoho Accounts (client id + client secret)\n      - Requested scopes granted by the Zoho Campaigns account owner\n    scopes_reference: scopes/zoho-campaigns-scopes.yml\n    source: https://www.zoho.com/campaigns/help/developers/access-token.html\n  - name: ZohoAPIKey\n    api: Zoho Campaigns Email API v2\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    value_format: 'Zoho-zapikey <api_key>'\n    scope: ZohoCampaigns.emailapi.ALL\n    key_limit: Maximum of 20 API keys per user\n    generation:\
  \ >-\n      Zoho Campaigns console -> API Keys -> Create API Key; name the key and\n      select the scope.\n    source: https://www.zoho.com/campaigns/help/emailapi/authentication.html\n  - name: ZohoOAuthEmailAPI\n    api: Zoho Campaigns Email API v1\n    type: oauth2\n    flow: authorizationCode\n    note: >-\n      The Email API v1 surface in the provider's own Postman collection is\n      grouped as \"v1 - OAuth\" and authenticates with the same Zoho Accounts\n      OAuth 2.0 tokens; v2 replaced it with the Zoho-zapikey API key above.\n    source: postman/zoho-campaigns-email-api-collection.json\nauthorization_server:\n  issuer: https://accounts.zoho.com\n  discovery: https://accounts.zoho.com/.well-known/openid-configuration\n  document: well-known/zoho-campaigns-openid-configuration.json\n  grant_types_supported:\n    - authorization_code\n    - implicit\n    - refresh_token\n    - 'urn:ietf:params:oauth:grant-type:device_code'\n    - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n\
  \  response_types_supported:\n    - code\n    - token\n  openid_scopes_supported:\n    - openid\n    - email\n    - profile\n    - phone\n  note: >-\n    The openid-configuration scopes_supported list carries only the OIDC\n    identity scopes. The Zoho Campaigns product scopes (ZohoCampaigns.*) are\n    published on the developer-guide page, not in discovery metadata.\ndata_centers:\n  note: >-\n    Zoho operates regional data centers (US, EU, IN, AU, JP, CA, CN, SA). Both\n    the accounts host and the campaigns host carry a region-specific TLD in\n    non-US regions (e.g. accounts.zoho.eu / campaigns.zoho.eu). The values above\n    are the US (.com) endpoints.\n  reference: https://accounts.zoho.com/oauth/serverinfo\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-campaigns/refs/heads/main/authentication/zoho-campaigns-authentication.yml
summary_line: oauth2/apiKey · 3 schemes
tags:
- Email Marketing
- Campaigns
- Mailing Lists
- Subscribers
- Email Templates
- A/B Testing
- Campaign Analytics
- Marketing Automation
- Transactional Email
- Webhooks
---
