---
anonymous_access: false
api_key_in: []
api_specs:
- filename: alviere-account-wallet-api-openapi.yml
  format: yaml
  label: ALVIERE Account Wallet API
  slug: alviere-account-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alviere/openapi/alviere-account-wallet-api-openapi.yml
- filename: alviere-accounts-api-openapi.yml
  format: yaml
  label: ALVIERE Accounts API
  slug: alviere-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alviere/openapi/alviere-accounts-api-openapi.yml
- filename: alviere-authentication-api-openapi.yml
  format: yaml
  label: ALVIERE Authentication API
  slug: alviere-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alviere/openapi/alviere-authentication-api-openapi.yml
- filename: alviere-bank-processing-api-openapi.yml
  format: yaml
  label: ALVIERE Bank Processing API
  slug: alviere-bank-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alviere/openapi/alviere-bank-processing-api-openapi.yml
- filename: alviere-card-issuance-api-openapi.yml
  format: yaml
  label: ALVIERE Card Issuance API
  slug: alviere-card-issuance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alviere/openapi/alviere-card-issuance-api-openapi.yml
- filename: alviere-card-processing-api-openapi.yml
  format: yaml
  label: ALVIERE Card Processing API
  slug: alviere-card-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alviere/openapi/alviere-card-processing-api-openapi.yml
- filename: alviere-remittances-api-openapi.yml
  format: yaml
  label: ALVIERE Remittances API
  slug: alviere-remittances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alviere/openapi/alviere-remittances-api-openapi.yml
- filename: alviere-reporting-api-openapi.yml
  format: yaml
  label: ALVIERE Reporting API
  slug: alviere-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alviere/openapi/alviere-reporting-api-openapi.yml
- filename: alviere-tokenization-api-openapi.yml
  format: yaml
  label: ALVIERE Tokenization API
  slug: alviere-tokenization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alviere/openapi/alviere-tokenization-api-openapi.yml
- filename: alviere-treasury-management-api-openapi.yml
  format: yaml
  label: ALVIERE Treasury Management API
  slug: alviere-treasury-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alviere/openapi/alviere-treasury-management-api-openapi.yml
auth_types: []
description: Authentication schemes as published on the Alviere documentation.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Alviere Authentication
name_suffix: Authentication
oauth_flows: []
overview: ALVIERE declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ALVIERE
provider_slug: alviere
scheme_count: 2
schemes:
- evidence: Alviere uses the OpenID authentication standard.
  how_to_obtain: Credentials (client_id and client_secret) are provided by your Program Manager; request them by emailing support@alviere.com.
  name: OpenID
  type: oauth2
- evidence: 'On all subsequent calls to the API, you''ll need to include a header in the HTTP request with that information. The format of the header is `Authorization: Bearer [your_access_token]`.'
  header: Authorization
  location: header
  name: Bearer Token
  type: http-bearer
slug: alviere-authentication
source_filename: alviere-authentication.yml
source_heading: Authentication Profile
source_url: https://apidocs.alviere.com/guides/integration/authentication/index.md
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://apidocs.alviere.com/guides/integration/authentication/index.md\nsources:\n- https://apidocs.alviere.com/guides/integration/authentication/index.md\ndescription: Authentication schemes as published on the Alviere documentation.\nschemes:\n- type: oauth2\n  name: OpenID\n  evidence: Alviere uses the OpenID authentication standard.\n  how_to_obtain: Credentials (client_id and client_secret) are provided by your Program Manager; request them by emailing support@alviere.com.\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'On all subsequent calls to the API, you''ll need to include a header in the HTTP request with that information. The format of the\n    header is `Authorization: Bearer [your_access_token]`.'\n  location: header\n  header: Authorization\ndocs: https://apidocs.alviere.com/guides/integration/authentication/index.md\n"
source_yaml_url: https://artifacts.apis.io/alviere/authentication/alviere-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Fintech
- Embedded Finance
- Banking
---
