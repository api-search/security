---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Coupa Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coupa Software secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Coupa Software
provider_slug: coupa-software
scheme_count: 2
schemes:
- description: OpenID Connect (an authentication layer on top of OAuth 2.0) is the required protocol for new Core API integrations. OIDC clients are created and managed within the Coupa instance administration (OpenID Connect Clients). Coupa documents OIDC client setup patterns for NetSuite OAuth and Okta user provisioning.
  name: OAuth2 / OIDC
  sources:
  - docs
  type: oauth2
- deprecated: true
  description: Legacy static API-key header authentication. Deprecated in favor of OAuth 2.0 / OIDC; remaining keys should be transitioned to OAuth clients and revoked.
  in: header
  name: API Key (deprecated)
  parameter: X-COUPA-API-KEY
  sources:
  - docs
  type: apiKey
slug: coupa-software-authentication
source_filename: coupa-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://compass.coupa.com/en-us/products/product-documentation/integration-technical-documentation/the-coupa-core-api/oauth-2.0-and-oidc\ndocs: https://compass.coupa.com/en-us/products/product-documentation/integration-technical-documentation/the-coupa-core-api/oauth-2.0-and-oidc\nsummary:\n  types: [oauth2, openIdConnect]\n  current: OAuth 2.0 / OpenID Connect (OIDC)\n  deprecated: [apiKey]\n  notes: >-\n    Coupa has transitioned the Core API from static API keys to OAuth 2.0 with OpenID Connect\n    (OIDC). API keys are deprecated: existing keys must be migrated to OAuth/OIDC clients and\n    revoked under Setup > API Keys. OAuth/OIDC clients are configured per Coupa instance.\nschemes:\n  - name: OAuth2 / OIDC\n    type: oauth2\n    description: >-\n      OpenID Connect (an authentication layer on top of OAuth 2.0) is the required protocol for\n      new Core API integrations. OIDC clients are created and managed within\
  \ the Coupa instance\n      administration (OpenID Connect Clients). Coupa documents OIDC client setup patterns for\n      NetSuite OAuth and Okta user provisioning.\n    sources: [docs]\n  - name: API Key (deprecated)\n    type: apiKey\n    in: header\n    parameter: X-COUPA-API-KEY\n    deprecated: true\n    description: >-\n      Legacy static API-key header authentication. Deprecated in favor of OAuth 2.0 / OIDC;\n      remaining keys should be transitioned to OAuth clients and revoked.\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coupa-software/refs/heads/main/authentication/coupa-software-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Procurement
- Spend Management
- Invoicing
- Expenses
- Payments
- Supply Chain
- Sourcing
- Contracts
- ERP
---
