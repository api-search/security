---
api_key_in:
- header
api_specs:
- filename: coupa-invoices-api-openapi.yml
  format: yaml
  label: Coupa Invoices API
  slug: coupa-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coupa/refs/heads/main/openapi/coupa-invoices-api-openapi.yml
- filename: coupa-purchase-orders-api-openapi.yml
  format: yaml
  label: Coupa Purchase Orders API
  slug: coupa-purchase-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coupa/refs/heads/main/openapi/coupa-purchase-orders-api-openapi.yml
- filename: coupa-requisitions-api-openapi.yml
  format: yaml
  label: Coupa Requisitions API
  slug: coupa-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coupa/refs/heads/main/openapi/coupa-requisitions-api-openapi.yml
- filename: coupa-suppliers-api-openapi.yml
  format: yaml
  label: Coupa Suppliers API
  slug: coupa-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coupa/refs/heads/main/openapi/coupa-suppliers-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Coupa Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Coupa secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Coupa
provider_slug: coupa
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication. Coupa supports the client_credentials grant type. Obtain client credentials from Coupa instance setup.
  flows:
  - flow: clientCredentials
    scopes: 8
    tokenUrl: https://{instance}.coupahost.com/oauth2/token
  name: oauth2
  sources:
  - openapi/coupa-core-api-openapi.yml
  type: oauth2
- description: Legacy API key authentication. Coupa recommends migrating to OAuth 2.0. API keys are configured per Coupa instance.
  in: header
  name: apiKey
  parameter: X-COUPA-API-KEY
  sources:
  - openapi/coupa-core-api-openapi.yml
  type: apiKey
slug: coupa-authentication
source_filename: coupa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coupa-core-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{instance}.coupahost.com/oauth2/token\n    scopes: 8\n  description: OAuth 2.0 authentication. Coupa supports the client_credentials grant type. Obtain\n    client credentials from Coupa instance setup.\n  sources:\n  - openapi/coupa-core-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-COUPA-API-KEY\n  description: Legacy API key authentication. Coupa recommends migrating to OAuth 2.0. API keys\n    are configured per Coupa instance.\n  sources:\n  - openapi/coupa-core-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coupa/refs/heads/main/authentication/coupa-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- BSM
- Business Spend Management
- Cloud Platform
- Enterprise
- Financial Management
- Invoicing
- Procurement
- Supply Chain
---
