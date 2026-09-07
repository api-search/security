---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: 7Learnings Authentication
name_suffix: Authentication
oauth_flows: []
overview: 7Learnings declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: 7Learnings
provider_slug: 7learnings
scheme_count: 3
schemes:
- bearer_methods_supported:
  - header
  client_registration: No RFC 7591 dynamic client registration endpoint is advertised. The authorization server sets client_id_metadata_document_supported = true, so a client identifies itself with a URL to a client-id metadata document rather than a pre-registered client_id.
  evidence: https://7learnings.com/.well-known/oauth-authorization-server
  evidence_status: 200
  flows:
    authorizationCode:
      authorizationUrl: https://7learnings.com/oauth/authorize
      refreshUrl: https://7learnings.com/oauth/token
      revocationUrl: https://7learnings.com/oauth/revoke
      scopes:
        mcp: Access the MCP server surface published by 7learnings.com
      tokenUrl: https://7learnings.com/oauth/token
  id: mcp_oauth2
  pkce_required_methods:
  - S256
  surface: https://7learnings.com/wp-json/mcp/mcp-oauth-server
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- detail: '"SSO and Multi-Factor Authentication (MFA) support" is stated on the security page; the 2026-08-06 changelog entry records that passwordless login and two-factor authentication are encouraged for app users.'
  evidence: https://7learnings.com/security-compliance-data-protection/
  evidence_status: 200
  id: steering_app_signin
  methods:
  - Single sign-on (SSO)
  - Multi-factor authentication (MFA)
  - Passwordless login
  surface: 7Learnings Steering App (customer web frontend)
  type: interactive
- detail: Each customer connection carries its own credentials for the underlying transport or vendor API - BigQuery, Snowflake, Microsoft Fabric, Google Cloud Storage, AWS S3, Azure Blob Storage, SFTP, FTPS, HTTPS, and the customer's Shopify, Tradebyte, Plentymarkets, commercetools, Scayle, Salesforce Commerce Cloud, Google Ads, Google Shopping, Google Analytics, Amazon SP-API and Amazon Ads accounts. No credential shapes, key prefixes or header names are published.
  evidence: https://app-static-7l.storage.googleapis.com/latest/7Learnings_initial_data_request.pdf
  evidence_status: 200
  id: customer_transport_credentials
  surface: data integration connectors (inbound and outbound)
  type: delegated
slug: 7learnings-authentication
source_filename: 7learnings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://7learnings.com/.well-known/oauth-authorization-server,\n  https://7learnings.com/.well-known/oauth-protected-resource,\n  https://7learnings.com/security-compliance-data-protection/,\n  https://7learnings.com/changelog/\nsummary: >-\n  7Learnings publishes no public REST API and therefore no OpenAPI securitySchemes. Two\n  authentication surfaces are nevertheless documented or observable: OAuth 2.0 on the MCP\n  endpoint served from 7learnings.com, and SSO/MFA/passwordless sign-in on the 7Learnings\n  Steering App. Customer data integration is authenticated per-connection, per-customer,\n  by the credentials of the transport (BigQuery/Snowflake/Fabric service accounts, cloud\n  object-store keys, SFTP/FTPS credentials, or the customer's own Shopify/Tradebyte/\n  Google Ads/Amazon SP-API tokens) - 7Learnings does not issue a public API key.\n\nschemes:\n- id: mcp_oauth2\n  type: oauth2\n  surface: https://7learnings.com/wp-json/mcp/mcp-oauth-server\n\
  \  flows:\n    authorizationCode:\n      authorizationUrl: https://7learnings.com/oauth/authorize\n      tokenUrl: https://7learnings.com/oauth/token\n      refreshUrl: https://7learnings.com/oauth/token\n      revocationUrl: https://7learnings.com/oauth/revoke\n      scopes:\n        mcp: Access the MCP server surface published by 7learnings.com\n  pkce_required_methods: [S256]\n  token_endpoint_auth_methods_supported: [none]\n  client_registration: >-\n    No RFC 7591 dynamic client registration endpoint is advertised. The authorization server\n    sets client_id_metadata_document_supported = true, so a client identifies itself with a\n    URL to a client-id metadata document rather than a pre-registered client_id.\n  bearer_methods_supported: [header]\n  evidence: https://7learnings.com/.well-known/oauth-authorization-server\n  evidence_status: 200\n\n- id: steering_app_signin\n  type: interactive\n  surface: 7Learnings Steering App (customer web frontend)\n  methods:\n  - Single sign-on\
  \ (SSO)\n  - Multi-factor authentication (MFA)\n  - Passwordless login\n  detail: >-\n    \"SSO and Multi-Factor Authentication (MFA) support\" is stated on the security page;\n    the 2026-08-06 changelog entry records that passwordless login and two-factor\n    authentication are encouraged for app users.\n  evidence: https://7learnings.com/security-compliance-data-protection/\n  evidence_status: 200\n\n- id: customer_transport_credentials\n  type: delegated\n  surface: data integration connectors (inbound and outbound)\n  detail: >-\n    Each customer connection carries its own credentials for the underlying transport or vendor\n    API - BigQuery, Snowflake, Microsoft Fabric, Google Cloud Storage, AWS S3, Azure Blob\n    Storage, SFTP, FTPS, HTTPS, and the customer's Shopify, Tradebyte, Plentymarkets,\n    commercetools, Scayle, Salesforce Commerce Cloud, Google Ads, Google Shopping, Google\n    Analytics, Amazon SP-API and Amazon Ads accounts. No credential shapes, key prefixes or\n\
  \    header names are published.\n  evidence: https://app-static-7l.storage.googleapis.com/latest/7Learnings_initial_data_request.pdf\n  evidence_status: 200\n\nkey_management:\n  customer_managed_encryption_keys: true\n  detail: >-\n    \"Customer-managed encryption keys, allowing clients the ability to immediately delete keys\n    to render data unreadable if necessary.\" Each client is deployed in a dedicated GCP project\n    with VPC Service Controls.\n  evidence: https://7learnings.com/security-compliance-data-protection/\n\nnot_found:\n- No public API key issuance or developer key management page\n- No /.well-known/openid-configuration (404)\n- No documented bearer/HTTP auth for a product REST API\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/7learnings/refs/heads/main/authentication/7learnings-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Retail
- Pricing
- Price Optimization
- Predictive Pricing
- Demand Forecasting
- Machine Learning
- Ecommerce
- Performance Marketing
- Data Integration
- Germany
- SaaS
---
