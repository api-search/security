---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ecosio-approval-request-status-api-openapi.yml
  format: yaml
  label: ecosio Approval Request Status API
  slug: ecosio-approval-request-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-approval-request-status-api-openapi.yml
- filename: ecosio-archive-messages-api-openapi.yml
  format: yaml
  label: ecosio Archive messages API
  slug: ecosio-archive-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-archive-messages-api-openapi.yml
- filename: ecosio-check-user-credentials-api-openapi.yml
  format: yaml
  label: ecosio Check user credentials API
  slug: ecosio-check-user-credentials-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-check-user-credentials-api-openapi.yml
- filename: ecosio-companies-api-openapi.yml
  format: yaml
  label: ecosio Companies API
  slug: ecosio-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-companies-api-openapi.yml
- filename: ecosio-connectors-api-openapi.yml
  format: yaml
  label: ecosio Connectors API
  slug: ecosio-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-connectors-api-openapi.yml
- filename: ecosio-deliver-messages-to-the-hub-api-openapi.yml
  format: yaml
  label: ecosio Deliver messages to the Hub API
  slug: ecosio-deliver-messages-to-the-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-deliver-messages-to-the-hub-api-openapi.yml
- filename: ecosio-fetch-messages-from-the-hub-api-openapi.yml
  format: yaml
  label: ecosio Fetch messages from the Hub API
  slug: ecosio-fetch-messages-from-the-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-fetch-messages-from-the-hub-api-openapi.yml
- filename: ecosio-message-controller-api-openapi.yml
  format: yaml
  label: ecosio Message Controller API
  slug: ecosio-message-controller-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-message-controller-api-openapi.yml
- filename: ecosio-request-the-documents-for-an-e-invoice-api-openapi.yml
  format: yaml
  label: ecosio Request the documents for an e-invoice API
  slug: ecosio-request-the-documents-for-an-e-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-request-the-documents-for-an-e-invoice-api-openapi.yml
- filename: ecosio-scenarios-api-openapi.yml
  format: yaml
  label: ecosio Scenarios API
  slug: ecosio-scenarios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecosio/openapi/ecosio-scenarios-api-openapi.yml
auth_types: []
description: Authentication methods for ecosio APIs including OAuth 2.0 client credentials and basic authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ecosio Authentication
name_suffix: Authentication
oauth_flows: []
overview: ecosio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ecosio
provider_slug: ecosio
scheme_count: 2
schemes:
- evidence: You can authenticate to the Management API using the OAuth 2.0 client credentials grant.
  flows:
  - client_credentials
  header: Authorization
  how_to_obtain: Retrieve the client ID and client secret for your Management API connector from the Monitor.
  location: header
  name: OAuth 2.0
  scopes:
  - management-api
  token_url: https://auth.ecosio-hub.com/oauth2/token
  type: oauth2
- evidence: You can authenticate to the Management API using basic authentication.
  header: Authorization
  how_to_obtain: You obtain these values in the Monitor.
  location: header
  name: Basic
  type: http-basic
slug: ecosio-authentication
source_filename: ecosio-authentication.yml
source_heading: Authentication Profile
source_url: https://connect.ecosio.com/reference/management-api-authentication
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (deepseek)\nsource: https://connect.ecosio.com/reference/management-api-authentication\nsources:\n- https://connect.ecosio.com/reference/management-api-authentication\n- https://connect.ecosio.com/reference/securitycredentials\n- https://connect.ecosio.com/reference/securitycredentials\n- https://connect.ecosio.com/reference/regeneratecredentials\ndescription: Authentication methods for ecosio APIs including OAuth 2.0 client credentials and basic authentication\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: You can authenticate to the Management API using the OAuth 2.0 client credentials grant.\n  flows:\n  - client_credentials\n  token_url: https://auth.ecosio-hub.com/oauth2/token\n  scopes:\n  - management-api\n  header: Authorization\n  location: header\n  how_to_obtain: Retrieve the client ID and client secret for your Management API connector from the Monitor.\n- type: http-basic\n\
  \  name: Basic\n  evidence: You can authenticate to the Management API using basic authentication.\n  header: Authorization\n  location: header\n  how_to_obtain: You obtain these values in the Monitor.\ndocs: https://connect.ecosio.com/reference/management-api-authentication\nnote: The basic authentication method is marked as deprecated. The OAuth 2.0 scheme also requires an additional X-APP-KEY header.\n"
source_yaml_url: https://artifacts.apis.io/ecosio/authentication/ecosio-authentication.yml
summary_line: 2 schemes
tags:
- Company
- EDI
- E-Invoicing
- B2B Integration
- VAT Compliance
- PEPPOL
- Supply Chain
- Messaging
---
