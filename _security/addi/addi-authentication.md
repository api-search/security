---
api_key_in: []
auth_types:
- oauth2
description: Addi's merchant credit/checkout API authenticates through Auth0 (Identity as a Service) using the OAuth2 client-credentials flow. Merchants receive a client_id ("Identificador del cliente") and client_secret ("Identificador secreto del cliente") — visible in the first-party VTEX/Magento/PrestaShop plugin configuration — and exchange them at the Auth0 token endpoint for a bearer access token that is presented on subsequent API calls. A separate sandbox ("Ambiente de Desarrollo") environment is used before switching to production.
kind: authentication
layout: security
method: searched
name: Addi Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Addi secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Addi
provider_slug: addi
scheme_count: 1
schemes:
- credentials:
    client_id: merchant client identifier (Identificador del cliente)
    client_secret: merchant client secret (Identificador secreto del cliente)
  environments:
  - docs: https://api-docs-sandbox.addi.com/auth/
    label: Ambiente de Desarrollo
    name: sandbox
  - api_host: https://api.addi.com
    name: production
  identity_provider: Auth0
  name: Auth0OAuth2
  scheme: clientCredentials
  sources:
  - docs
  - packages/addi-packages.yml
  token_presentation: Bearer access token in Authorization header
  type: oauth2
slug: addi-authentication
source_filename: addi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://api-docs-sandbox.addi.com/auth/\ndocs: https://api-docs-sandbox.addi.com/auth/\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  identity_provider: Auth0\ndescription: >-\n  Addi's merchant credit/checkout API authenticates through Auth0 (Identity as a\n  Service) using the OAuth2 client-credentials flow. Merchants receive a client_id\n  (\"Identificador del cliente\") and client_secret (\"Identificador secreto del\n  cliente\") — visible in the first-party VTEX/Magento/PrestaShop plugin\n  configuration — and exchange them at the Auth0 token endpoint for a bearer\n  access token that is presented on subsequent API calls. A separate sandbox\n  (\"Ambiente de Desarrollo\") environment is used before switching to production.\nschemes:\n- name: Auth0OAuth2\n  type: oauth2\n  scheme: clientCredentials\n  identity_provider: Auth0\n  credentials:\n    client_id: merchant client identifier (Identificador\
  \ del cliente)\n    client_secret: merchant client secret (Identificador secreto del cliente)\n  token_presentation: Bearer access token in Authorization header\n  environments:\n  - name: sandbox\n    label: Ambiente de Desarrollo\n    docs: https://api-docs-sandbox.addi.com/auth/\n  - name: production\n    api_host: https://api.addi.com\n  sources: [docs, packages/addi-packages.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/addi/refs/heads/main/authentication/addi-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Fintech
- Payments
- Buy Now Pay Later
- Credit
- Lending
- Checkout
- E-commerce
- Latin America
- Colombia
---
