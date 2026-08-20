---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Backstory Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Backstory secures its APIs with oauth2, apiKey, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Backstory
provider_slug: backstory
scheme_count: 4
schemes:
- applies_to: Backstory MCP (https://mcp.people.ai/mcp)
  bearer_methods:
  - header
  flows:
  - authorizationUrl: https://mcp.backstory.ai/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    issuer: https://mcp.backstory.ai/
    registrationUrl: https://mcp.backstory.ai/register
    revocationUrl: https://mcp.backstory.ai/revoke
    scopes:
      claudeai: The only scope advertised in the server's RFC 8414 metadata. The provider publishes no scope reference; per the docs, authorization is not scope-shaped at all — a token inherits the signing-in user's own Backstory record permissions.
    tokenUrl: https://mcp.backstory.ai/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
  name: backstory-mcp-oauth2
  sources:
  - https://mcp.backstory.ai/.well-known/oauth-authorization-server
  - https://mcp.backstory.ai/.well-known/oauth-protected-resource/mcp
  - https://help.backstory.ai/en/articles/15252710-connect-claude-to-backstory
  type: oauth2
- applies_to: Backstory MCP, programmatic clients (documented for n8n)
  case_sensitive: true
  in: header
  issuance: Issued on request by a Backstory administrator or Customer Success Manager. No self-service issuance is documented.
  name: pai-client-credentials
  names:
  - PAI-Client-Id
  - PAI-Client-Secret
  sources:
  - https://help.backstory.ai/en/articles/15252917-connect-n8n-to-backstory
  type: apiKey
- applies_to: Backstory REST API
  in: unknown
  issuance: Backstory administrators generate, pause and revoke API key/secret pairs on the API Keys page of the Backstory Admin Panel; a maximum of five active pairs per organization. The transport, header name and base URL for the REST API are not published — the help centre documents key lifecycle only.
  name: backstory-rest-api-key
  sources:
  - https://help.backstory.ai/en/articles/15252717-api-key-management
  type: apiKey
- applies_to: Backstory web application and Salesforce-embedded surfaces
  name: salesforce-sso-saml
  note: The product application authenticates through Salesforce OAuth/SSO and honours the customer's SAML IdP (Okta documented). As of the August 2026 release, Backstory MCP no longer requires Salesforce credentials and accepts Backstory credentials directly; enterprise IdP pass-through (Okta, Entra ID) is available on request.
  scheme: sso
  sources:
  - https://help.backstory.ai/en/articles/15252780-single-sign-on
  - https://help.backstory.ai/en/articles/15252889-common-security-and-privacy-questions
  - https://help.backstory.ai/en/articles/15252920-new-product-releases
  type: http
slug: backstory-authentication
source_filename: backstory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://help.backstory.ai/en/articles/15252736-backstory-mcp\ndocs: https://help.backstory.ai/en/collections/19658946-mcp\nnote: >-\n  Derived from the provider's own help-centre documentation plus live\n  unauthenticated probes of the MCP host. There is no OpenAPI for Backstory, so\n  none of this comes from a securitySchemes block — every scheme below was read\n  off a published setup article or an observed HTTP response.\nsummary:\n  types: [oauth2, apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  dynamic_client_registration: true\n  pkce: required\nschemes:\n- name: backstory-mcp-oauth2\n  type: oauth2\n  applies_to: Backstory MCP (https://mcp.people.ai/mcp)\n  flows:\n  - flow: authorizationCode\n    issuer: https://mcp.backstory.ai/\n    authorizationUrl: https://mcp.backstory.ai/authorize\n    tokenUrl: https://mcp.backstory.ai/token\n    revocationUrl: https://mcp.backstory.ai/revoke\n \
  \   registrationUrl: https://mcp.backstory.ai/register\n    grant_types: [authorization_code, refresh_token]\n    code_challenge_methods: [S256]\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n    scopes:\n      claudeai: >-\n        The only scope advertised in the server's RFC 8414 metadata. The\n        provider publishes no scope reference; per the docs, authorization is\n        not scope-shaped at all — a token inherits the signing-in user's own\n        Backstory record permissions.\n  bearer_methods: [header]\n  sources:\n  - https://mcp.backstory.ai/.well-known/oauth-authorization-server\n  - https://mcp.backstory.ai/.well-known/oauth-protected-resource/mcp\n  - https://help.backstory.ai/en/articles/15252710-connect-claude-to-backstory\n- name: pai-client-credentials\n  type: apiKey\n  in: header\n  names: [PAI-Client-Id, PAI-Client-Secret]\n  case_sensitive: true\n  applies_to: Backstory MCP, programmatic clients (documented for n8n)\n  issuance:\
  \ >-\n    Issued on request by a Backstory administrator or Customer Success Manager.\n    No self-service issuance is documented.\n  sources:\n  - https://help.backstory.ai/en/articles/15252917-connect-n8n-to-backstory\n- name: backstory-rest-api-key\n  type: apiKey\n  applies_to: Backstory REST API\n  issuance: >-\n    Backstory administrators generate, pause and revoke API key/secret pairs on\n    the API Keys page of the Backstory Admin Panel; a maximum of five active\n    pairs per organization. The transport, header name and base URL for the REST\n    API are not published — the help centre documents key lifecycle only.\n  in: unknown\n  sources:\n  - https://help.backstory.ai/en/articles/15252717-api-key-management\n- name: salesforce-sso-saml\n  type: http\n  scheme: sso\n  applies_to: Backstory web application and Salesforce-embedded surfaces\n  note: >-\n    The product application authenticates through Salesforce OAuth/SSO and\n    honours the customer's SAML IdP (Okta documented).\
  \ As of the August 2026\n    release, Backstory MCP no longer requires Salesforce credentials and accepts\n    Backstory credentials directly; enterprise IdP pass-through (Okta, Entra ID)\n    is available on request.\n  sources:\n  - https://help.backstory.ai/en/articles/15252780-single-sign-on\n  - https://help.backstory.ai/en/articles/15252889-common-security-and-privacy-questions\n  - https://help.backstory.ai/en/articles/15252920-new-product-releases\nauthorization_model:\n  style: user-permission-inheritance\n  description: >-\n    Backstory MCP grants no privileges of its own. A connected AI client can read\n    exactly the accounts, opportunities, activities and other records the\n    authenticating user can already see in Backstory Engagement Dashboards;\n    administrators control that through User Access / Object Visibility settings.\n  source: https://help.backstory.ai/en/articles/15252736-backstory-mcp\nobserved_challenge:\n  url: https://mcp.people.ai/mcp\n  http_status:\
  \ 401\n  www_authenticate: >-\n    Bearer error=\"invalid_token\", error_description=\"Authentication failed. The\n    provided bearer token is invalid, expired, or no longer recognized by the\n    server...\", resource_metadata=\"https://mcp.backstory.ai/.well-known/oauth-protected-resource/mcp\"\n  fetched: '2026-08-14'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/backstory/refs/heads/main/authentication/backstory-authentication.yml
summary_line: oauth2/apiKey/http · 4 schemes
tags:
- Company
- Artificial Intelligence
- Revenue Intelligence
- Sales
- CRM
- Sales Analytics
- Forecasting
- Revenue Operations
- MCP
- AI Agents
---
