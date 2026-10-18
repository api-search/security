---
anonymous_access: false
api_key_in: []
api_specs:
- filename: contactout-api-usage-stats-api-openapi.yml
  format: yaml
  label: ContactOut API Usage Stats API
  slug: contactout-api-usage-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-api-usage-stats-api-openapi.yml
- filename: contactout-campaigns-api-api-openapi.yml
  format: yaml
  label: ContactOut Campaigns API
  slug: contactout-campaigns-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-campaigns-api-api-openapi.yml
- filename: contactout-company-information-from-domains-api-openapi.yml
  format: yaml
  label: ContactOut Company information from domains API
  slug: contactout-company-information-from-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-company-information-from-domains-api-openapi.yml
- filename: contactout-company-search-api-api-openapi.yml
  format: yaml
  label: ContactOut Company Search API
  slug: contactout-company-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-company-search-api-api-openapi.yml
- filename: contactout-contact-checker-api-api-openapi.yml
  format: yaml
  label: ContactOut Contact Checker API
  slug: contactout-contact-checker-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-contact-checker-api-api-openapi.yml
- filename: contactout-contact-info-api-bulk-api-openapi.yml
  format: yaml
  label: ContactOut Contact Info API - Bulk API
  slug: contactout-contact-info-api-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-contact-info-api-bulk-api-openapi.yml
- filename: contactout-contact-info-api-single-api-openapi.yml
  format: yaml
  label: ContactOut Contact Info API - Single API
  slug: contactout-contact-info-api-single-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-contact-info-api-single-api-openapi.yml
- filename: contactout-decision-makers-api-api-openapi.yml
  format: yaml
  label: ContactOut Decision Makers API
  slug: contactout-decision-makers-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-decision-makers-api-api-openapi.yml
- filename: contactout-email-to-linkedin-api-api-openapi.yml
  format: yaml
  label: ContactOut Email to LinkedIn API
  slug: contactout-email-to-linkedin-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-email-to-linkedin-api-api-openapi.yml
- filename: contactout-email-verifier-api-api-openapi.yml
  format: yaml
  label: ContactOut Email Verifier API
  slug: contactout-email-verifier-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-email-verifier-api-api-openapi.yml
- filename: contactout-hashed-email-api-api-openapi.yml
  format: yaml
  label: ContactOut Hashed Email API
  slug: contactout-hashed-email-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-hashed-email-api-api-openapi.yml
- filename: contactout-linkedin-profile-api-api-openapi.yml
  format: yaml
  label: ContactOut LinkedIn Profile API
  slug: contactout-linkedin-profile-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-linkedin-profile-api-api-openapi.yml
- filename: contactout-people-count-api-api-openapi.yml
  format: yaml
  label: ContactOut People Count API
  slug: contactout-people-count-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-people-count-api-api-openapi.yml
- filename: contactout-people-enrich-api-api-openapi.yml
  format: yaml
  label: ContactOut People Enrich API
  slug: contactout-people-enrich-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-people-enrich-api-api-openapi.yml
- filename: contactout-people-search-api-api-openapi.yml
  format: yaml
  label: ContactOut People Search API
  slug: contactout-people-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/openapi/contactout-people-search-api-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Contactout Authentication
name_suffix: Authentication
oauth_flows: []
overview: ContactOut declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ContactOut
provider_slug: contactout
scheme_count: 2
schemes:
- description: 'ContactOut uses API keys to allow access to the API. You can request an API key by booking a meeting. ContactOut expects the API key to be included in all API requests to the server in a header that looks like the following: token : <YOUR_API_TOKEN>'
  example_headers:
  - 'authorization: basic'
  - 'token: <YOUR_API_TOKEN>'
  in: header
  name: apiToken
  obtain: https://contactout.com/meeting?utm_source=api_docs
  parameter: token
  surfaces:
  - REST API
  type: apiKey
- dynamic_client_registration: https://contactout.com/api-users/oauth/register
  flows:
    authorizationCode:
      authorizationUrl: https://contactout.com/api-users/oauth/authorize
      refreshUrl: https://contactout.com/api-users/oauth/token
      scopes:
        mcp:use: Use the ContactOut MCP server
      tokenUrl: https://contactout.com/api-users/oauth/token
  metadata: https://contactout.com/.well-known/oauth-authorization-server
  name: mcpOAuth
  pkce: S256
  surfaces:
  - MCP server https://contactout.com/mcp
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: contactout-authentication
source_filename: contactout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource:\n- https://api.contactout.com#authentication\n- https://contactout.com/.well-known/oauth-authorization-server\ndocs: https://api.contactout.com#authentication\nsummary: 'REST API: an API key sent in a custom \"token\" request header on every request (the curl example also sends \"authorization: basic\"). Keys are issued by ContactOut after booking a meeting. The hosted MCP server uses OAuth 2.0 authorization code with PKCE, completed with the same API token.'\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  parameter: token\n  description: 'ContactOut uses API keys to allow access to the API. You can request an API key by booking a meeting. ContactOut expects the API key to be included in all API requests to the server in a header that looks like the following: token : <YOUR_API_TOKEN>'\n  example_headers:\n  - 'authorization: basic'\n  - 'token: <YOUR_API_TOKEN>'\n  surfaces: [REST API]\n  obtain: https://contactout.com/meeting?utm_source=api_docs\n\
  - name: mcpOAuth\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://contactout.com/api-users/oauth/authorize\n      tokenUrl: https://contactout.com/api-users/oauth/token\n      refreshUrl: https://contactout.com/api-users/oauth/token\n      scopes:\n        mcp:use: Use the ContactOut MCP server\n  pkce: S256\n  dynamic_client_registration: https://contactout.com/api-users/oauth/register\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  metadata: https://contactout.com/.well-known/oauth-authorization-server\n  surfaces: [MCP server https://contactout.com/mcp]\nnotes:\n- 'The ai-info page (https://contactout.com/ai-info) summarises authentication as \"Authorization: Bearer\"; the API reference, which is the developer source, documents the token header shown above.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contactout/refs/heads/main/authentication/contactout-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Contact Data
- Email Finder
- Data Enrichment
- People Search
- Company Search
- Email Verification
- Sales Intelligence
- Recruiting
- B2B Data
---
