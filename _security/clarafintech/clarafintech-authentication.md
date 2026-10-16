---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clarafintech-accounts-payable-api-openapi.yml
  format: yaml
  label: Clarafintech Accounts Payable API
  slug: clarafintech-accounts-payable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-accounts-payable-api-openapi.yml
- filename: clarafintech-authentication-api-openapi.yml
  format: yaml
  label: Clarafintech Authentication API
  slug: clarafintech-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-authentication-api-openapi.yml
- filename: clarafintech-billing-statements-api-openapi.yml
  format: yaml
  label: Clarafintech Billing Statements API
  slug: clarafintech-billing-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-billing-statements-api-openapi.yml
- filename: clarafintech-cards-api-openapi.yml
  format: yaml
  label: Clarafintech Cards API
  slug: clarafintech-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-cards-api-openapi.yml
- filename: clarafintech-digital-account-api-openapi.yml
  format: yaml
  label: Clarafintech Digital Account API
  slug: clarafintech-digital-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-digital-account-api-openapi.yml
- filename: clarafintech-extracted-documents-api-openapi.yml
  format: yaml
  label: Clarafintech Extracted Documents API
  slug: clarafintech-extracted-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-extracted-documents-api-openapi.yml
- filename: clarafintech-invoices-api-openapi.yml
  format: yaml
  label: Clarafintech Invoices API
  slug: clarafintech-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-invoices-api-openapi.yml
- filename: clarafintech-reimbursements-api-openapi.yml
  format: yaml
  label: Clarafintech Reimbursements API
  slug: clarafintech-reimbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-reimbursements-api-openapi.yml
- filename: clarafintech-transactions-api-openapi.yml
  format: yaml
  label: Clarafintech Transactions API
  slug: clarafintech-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-transactions-api-openapi.yml
- filename: clarafintech-users-api-openapi.yml
  format: yaml
  label: Clarafintech Users API
  slug: clarafintech-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/openapi/clarafintech-users-api-openapi.yml
auth_types: []
description: 'Clara API uses two‑layer authentication: mutual TLS (mTLS) for the connection and OAuth 2.0 Bearer token for each request. Both must be present.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Clarafintech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clarafintech declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Clarafintech
provider_slug: clarafintech
scheme_count: 2
schemes:
- evidence: 'Clara’s API uses two-layer authentication: mTLS (mutual TLS) for the connection and OAuth 2.0 Bearer token for each request.'
  how_to_obtain: Create a project in the Clara dashboard and download the client certificate (public key) and private key; the certificate is used during the TLS handshake.
  name: mutual TLS
  type: mtls
- evidence: 'Each HTTP request must include an Authorization: Bearer <token> header. Tokens are short‑lived JWTs obtained from the /oauth/token endpoint using your client_id and client_secret.'
  header: Authorization
  how_to_obtain: 'Use your client certificate, private key, client_id, and client_secret to POST to the token endpoint (e.g., curl --request POST "https://public-api.mx.clara.com/oauth/token" --header "Authorization: Basic $( echo -n ''CLIENT_ID:CLIENT_SECRET'' | base64 )" --cert client.crt --key client.key).'
  location: header
  name: OAuth 2.0 Bearer token
  token_url: https://public-api.mx.clara.com/oauth/token
  type: oauth2
slug: clarafintech-authentication
source_filename: clarafintech-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.clara.team/authentication
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.clara.team/authentication\nsources:\n- https://developers.clara.team/authentication\ndescription: 'Clara API uses two‑layer authentication: mutual TLS (mTLS) for the connection and OAuth 2.0 Bearer token for each request. Both\n  must be present.'\nschemes:\n- type: mtls\n  name: mutual TLS\n  evidence: 'Clara’s API uses two-layer authentication: mTLS (mutual TLS) for the connection and OAuth 2.0 Bearer token for each request.'\n  how_to_obtain: Create a project in the Clara dashboard and download the client certificate (public key) and private key; the certificate is\n    used during the TLS handshake.\n- type: oauth2\n  name: OAuth 2.0 Bearer token\n  evidence: 'Each HTTP request must include an Authorization: Bearer <token> header. Tokens are short‑lived JWTs obtained from the /oauth/token\n    endpoint using your client_id and client_secret.'\n  location:\
  \ header\n  header: Authorization\n  token_url: https://public-api.mx.clara.com/oauth/token\n  how_to_obtain: 'Use your client certificate, private key, client_id, and client_secret to POST to the token endpoint (e.g., curl --request POST\n    \"https://public-api.mx.clara.com/oauth/token\" --header \"Authorization: Basic $( echo -n ''CLIENT_ID:CLIENT_SECRET'' | base64 )\" --cert client.crt\n    --key client.key).'\ndocs: https://developers.clara.team/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clarafintech/refs/heads/main/authentication/clarafintech-authentication.yml
summary_line: 2 schemes
tags:
- Fintech
- Spend Management
- Latin America
- Corporate Cards
- Financial Automation
- Company
---
