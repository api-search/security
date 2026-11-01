---
anonymous_access: false
api_key_in: []
api_specs:
- filename: notarize-com-cost-centers-api-openapi.yml
  format: yaml
  label: Notarize Cost Centers API
  slug: notarize-com-cost-centers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-cost-centers-api-openapi.yml
- filename: notarize-com-documents-api-openapi.yml
  format: yaml
  label: Notarize Documents API
  slug: notarize-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-documents-api-openapi.yml
- filename: notarize-com-eligibilities-api-openapi.yml
  format: yaml
  label: Notarize Eligibilities API
  slug: notarize-com-eligibilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-eligibilities-api-openapi.yml
- filename: notarize-com-enote-api-openapi.yml
  format: yaml
  label: Notarize E Note API
  slug: notarize-com-enote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-enote-api-openapi.yml
- filename: notarize-com-integrations-api-openapi.yml
  format: yaml
  label: Notarize Integrations API
  slug: notarize-com-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-integrations-api-openapi.yml
- filename: notarize-com-notaries-api-openapi.yml
  format: yaml
  label: Notarize Notaries API
  slug: notarize-com-notaries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-notaries-api-openapi.yml
- filename: notarize-com-notarization-records-api-openapi.yml
  format: yaml
  label: Notarize Notarization Records API
  slug: notarize-com-notarization-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-notarization-records-api-openapi.yml
- filename: notarize-com-oauth-2-0-api-openapi.yml
  format: yaml
  label: Notarize OAuth 2.0 API
  slug: notarize-com-oauth-2-0-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-oauth-2-0-api-openapi.yml
- filename: notarize-com-oid4vp-api-openapi.yml
  format: yaml
  label: Notarize OID4VP API
  slug: notarize-com-oid4vp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-oid4vp-api-openapi.yml
- filename: notarize-com-organizations-api-openapi.yml
  format: yaml
  label: Notarize Organizations API
  slug: notarize-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-organizations-api-openapi.yml
- filename: notarize-com-referrals-api-openapi.yml
  format: yaml
  label: Notarize Referrals API
  slug: notarize-com-referrals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-referrals-api-openapi.yml
- filename: notarize-com-scim-api-openapi.yml
  format: yaml
  label: Notarize SCIM API
  slug: notarize-com-scim-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-scim-api-openapi.yml
- filename: notarize-com-security-events-api-openapi.yml
  format: yaml
  label: Notarize Security Events API
  slug: notarize-com-security-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-security-events-api-openapi.yml
- filename: notarize-com-templates-api-openapi.yml
  format: yaml
  label: Notarize Templates API
  slug: notarize-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-templates-api-openapi.yml
- filename: notarize-com-title-agencies-api-openapi.yml
  format: yaml
  label: Notarize Title Agencies API
  slug: notarize-com-title-agencies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-title-agencies-api-openapi.yml
- filename: notarize-com-transactions-api-openapi.yml
  format: yaml
  label: Notarize Transactions API
  slug: notarize-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-transactions-api-openapi.yml
- filename: notarize-com-webhooks-api-openapi.yml
  format: yaml
  label: Notarize Webhooks API
  slug: notarize-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notarize-com/openapi/notarize-com-webhooks-api-openapi.yml
auth_types: []
description: 'Proof API supports two authentication methods: API keys passed in the `ApiKey` request header, and OAuth 2.0 client‑credentials flow where a token is obtained via a Basic‑auth request to the token endpoint and then sent in a Bearer‑auth header.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Notarize Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Notarize declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Notarize
provider_slug: notarize-com
scheme_count: 2
schemes:
- evidence: "Authentication is simple - just include your key in the request header with the following format:\n\n```\nHeaders {\nApiKey: {YOUR API KEY HERE} \nContent-Type: application/json\n}\n```"
  header: ApiKey
  how_to_obtain: Create a Production or Fairfax API key in Settings >> API Keys of your Business Account.
  location: header
  name: ApiKey
  type: apiKey
- evidence: The Proof API supports the use of the `client_credentials` grant type as an alternative form of authentication, as defined under the OAuth 2.0 specification.
  flows:
  - client_credentials
  how_to_obtain: Provision a client application in Settings >> OAuth settings, then use the client_id and client_secret (provided once) to request a token.
  name: OAuth2 Client Credentials
  scopes:
  - read
  - write
  token_url: https://api.proof.com/oauth/v2/token
  type: oauth2
slug: notarize-com-authentication
source_filename: notarize-com-authentication.yml
source_heading: Authentication Profile
source_url: https://dev.proof.com/docs/api-keys.md
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dev.proof.com/docs/api-keys.md\nsources:\n- https://dev.proof.com/docs/api-keys.md\n- https://dev.proof.com/docs/oauth-client-credentials.md\n- https://dev.proof.com/docs/proof-api-keys-and-secret-scanning.md\n- https://dev.proof.com/docs/digital-credentials-overview.md\ndescription: 'Proof API supports two authentication methods: API keys passed in the `ApiKey` request header, and OAuth 2.0 client‑credentials\n  flow where a token is obtained via a Basic‑auth request to the token endpoint and then sent in a Bearer‑auth header.'\nschemes:\n- type: apiKey\n  name: ApiKey\n  evidence: \"Authentication is simple - just include your key in the request header with the following format:\\n\\n```\\nHeaders {\\nApiKey: {YOUR\\\n    \\ API KEY HERE} \\nContent-Type: application/json\\n}\\n```\"\n  location: header\n  header: ApiKey\n  how_to_obtain: Create a Production or Fairfax\
  \ API key in Settings >> API Keys of your Business Account.\n- type: oauth2\n  name: OAuth2 Client Credentials\n  evidence: The Proof API supports the use of the `client_credentials` grant type as an alternative form of authentication, as defined under the\n    OAuth 2.0 specification.\n  flows:\n  - client_credentials\n  token_url: https://api.proof.com/oauth/v2/token\n  scopes:\n  - read\n  - write\n  how_to_obtain: Provision a client application in Settings >> OAuth settings, then use the client_id and client_secret (provided once) to request\n    a token.\ndocs: https://dev.proof.com/docs/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/notarize-com/authentication/notarize-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Notarization
- LegalTech
- SaaS
- DigitalSignature
---
