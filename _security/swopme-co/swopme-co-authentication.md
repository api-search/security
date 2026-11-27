---
anonymous_access: false
api_key_in: []
api_specs:
- filename: swopme-co-control-api-openapi.yml
  format: yaml
  label: Swop Control API
  slug: swopme-co-control-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-control-api-openapi.yml
- filename: swopme-co-oidc-api-openapi.yml
  format: yaml
  label: Swop Oidc API
  slug: swopme-co-oidc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-oidc-api-openapi.yml
- filename: swopme-co-runtime-accounts-api-openapi.yml
  format: yaml
  label: Swop Runtime Accounts API
  slug: swopme-co-runtime-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-runtime-accounts-api-openapi.yml
- filename: swopme-co-runtime-auth-api-openapi.yml
  format: yaml
  label: Swop Runtime Auth API
  slug: swopme-co-runtime-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-runtime-auth-api-openapi.yml
- filename: swopme-co-runtime-intents-api-openapi.yml
  format: yaml
  label: Swop Runtime Intents API
  slug: swopme-co-runtime-intents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-runtime-intents-api-openapi.yml
- filename: swopme-co-runtime-session-grants-api-openapi.yml
  format: yaml
  label: Swop Runtime Session Grants API
  slug: swopme-co-runtime-session-grants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-runtime-session-grants-api-openapi.yml
- filename: swopme-co-runtime-sponsorship-api-openapi.yml
  format: yaml
  label: Swop Runtime Sponsorship API
  slug: swopme-co-runtime-sponsorship-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-runtime-sponsorship-api-openapi.yml
- filename: swopme-co-server-users-api-openapi.yml
  format: yaml
  label: Swop Server Users API
  slug: swopme-co-server-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-server-users-api-openapi.yml
- filename: swopme-co-server-wallets-api-openapi.yml
  format: yaml
  label: Swop Server Wallets API
  slug: swopme-co-server-wallets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-server-wallets-api-openapi.yml
- filename: swopme-co-server-webhooks-api-openapi.yml
  format: yaml
  label: Swop Server Webhooks API
  slug: swopme-co-server-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-server-webhooks-api-openapi.yml
- filename: swopme-co-system-api-openapi.yml
  format: yaml
  label: Swop System API
  slug: swopme-co-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/swopme-co/openapi/swopme-co-system-api-openapi.yml
auth_types: []
description: Authentication methods for Swop APIs as documented.
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Swop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swop declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Swop
provider_slug: swopme-co
scheme_count: 5
schemes:
- evidence: 'Use either header: Authorization header X-API-Key header'
  header: X-API-Key
  how_to_obtain: Create a merchant API key in the Swop web app Dashboard → Developer; the secret starts with swop_sk_ and is shown once.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Method Example Use when Header x-project-secret: YOUR_PROJECT_SECRET'
  header: x-project-secret
  how_to_obtain: Request access to Swop RPC preview; a project secret is provided for the project.
  location: header
  name: x-project-secret
  type: apiKey
- evidence: 'Basic auth Authorization: Basic base64(projectId:secret)'
  header: Authorization
  how_to_obtain: Request access to Swop RPC preview; a project secret is provided for the project.
  location: header
  name: Basic
  type: http-basic
- evidence: Query parameter ?projectSecret=YOUR_PROJECT_SECRET
  how_to_obtain: Request access to Swop RPC preview; a project secret is provided for the project.
  location: query
  name: projectSecret query
  type: apiKey
- evidence: 'Auth: x-swivy-app-id + x-swivy-publishable-key or x-swivy-app-id + x-swivy-secret-key'
  header: x-swivy-app-id, x-swivy-publishable-key
  how_to_obtain: Obtain Swivy app credentials by creating a Swivy project and receiving the app ID and publishable or secret key.
  location: header
  name: x-swivy-app-id & x-swivy-publishable-key
  type: apiKey
slug: swopme-co-authentication
source_filename: swopme-co-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.swopme.co/api-reference/authentication
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.swopme.co/api-reference/authentication\nsources:\n- https://docs.swopme.co/api-reference/authentication\n- https://docs.swopme.co/get-started/authentication\n- https://docs.swopme.co/rpc/authentication\n- https://docs.swopme.co/swivy/api-reference/auth\ndescription: Authentication methods for Swop APIs as documented.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Use either header: Authorization header X-API-Key header'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a merchant API key in the Swop web app Dashboard → Developer; the secret starts with swop_sk_ and is shown once.\n- type: apiKey\n  name: x-project-secret\n  evidence: 'Method Example Use when Header x-project-secret: YOUR_PROJECT_SECRET'\n  location: header\n  header: x-project-secret\n  how_to_obtain: Request access to Swop RPC preview; a project secret is provided for the\
  \ project.\n- type: http-basic\n  name: Basic\n  evidence: 'Basic auth Authorization: Basic base64(projectId:secret)'\n  location: header\n  header: Authorization\n  how_to_obtain: Request access to Swop RPC preview; a project secret is provided for the project.\n- type: apiKey\n  name: projectSecret query\n  evidence: Query parameter ?projectSecret=YOUR_PROJECT_SECRET\n  location: query\n  how_to_obtain: Request access to Swop RPC preview; a project secret is provided for the project.\n- type: apiKey\n  name: x-swivy-app-id & x-swivy-publishable-key\n  evidence: 'Auth: x-swivy-app-id + x-swivy-publishable-key or x-swivy-app-id + x-swivy-secret-key'\n  location: header\n  header: x-swivy-app-id, x-swivy-publishable-key\n  how_to_obtain: Obtain Swivy app credentials by creating a Swivy project and receiving the app ID and publishable or secret key.\ndocs: https://docs.swopme.co/api-reference/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/swopme-co/authentication/swopme-co-authentication.yml
summary_line: 5 schemes
tags:
- FinTech
- Identity
- Payments
- AI
- Wallet
---
