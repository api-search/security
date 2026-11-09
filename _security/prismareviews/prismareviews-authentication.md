---
anonymous_access: false
api_key_in: []
api_specs:
- filename: prismareviews-connections-api-openapi.yml
  format: yaml
  label: Prisma Reviews Connections API
  slug: prismareviews-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-connections-api-openapi.yml
- filename: prismareviews-locations-api-openapi.yml
  format: yaml
  label: Prisma Reviews Locations API
  slug: prismareviews-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-locations-api-openapi.yml
- filename: prismareviews-platforms-api-openapi.yml
  format: yaml
  label: Prisma Reviews Platforms API
  slug: prismareviews-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-platforms-api-openapi.yml
- filename: prismareviews-replies-api-openapi.yml
  format: yaml
  label: Prisma Reviews Replies API
  slug: prismareviews-replies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-replies-api-openapi.yml
- filename: prismareviews-reviews-api-openapi.yml
  format: yaml
  label: Prisma Reviews Reviews API
  slug: prismareviews-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-reviews-api-openapi.yml
- filename: prismareviews-stats-api-openapi.yml
  format: yaml
  label: Prisma Reviews Stats API
  slug: prismareviews-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-stats-api-openapi.yml
- filename: prismareviews-usage-api-openapi.yml
  format: yaml
  label: Prisma Reviews Usage API
  slug: prismareviews-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-usage-api-openapi.yml
- filename: prismareviews-webhooks-api-openapi.yml
  format: yaml
  label: Prisma Reviews Webhooks API
  slug: prismareviews-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prismareviews/openapi/prismareviews-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods described in the Prisma Reviews documentation
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Prismareviews Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prisma Reviews declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Prisma Reviews
provider_slug: prismareviews
scheme_count: 3
schemes:
- evidence: Every request to https://api.prismareviews.com/v1 needs an API key in the Authorization header, as a Bearer token.
  header: Authorization
  how_to_obtain: Get a live key and a test key from the Prisma dashboard after creating an account.
  location: header
  name: Prisma API Key
  type: http-bearer
- evidence: 'Token requests authenticate with Authorization: Basic base64(API_KEY:API_SECRET) . For client credentials ( grant docs ):'
  flows:
  - client_credentials
  header: Authorization
  how_to_obtain: Create an API application in Trustpilot Business to obtain the API key and secret, then request a token using the client_credentials grant.
  location: header
  name: Trustpilot OAuth2
  token_url: https://api.trustpilot.com/v1/oauth/oauth-business-users-for-applications/accesstoken
  type: oauth2
- evidence: Every request to the App Store Connect API carries a JSON Web Token signed with the .p8 key (algorithm ES256), with the Key ID in the header, the Issuer ID as iss and an expiry of at most 20 minutes for the reviews endpoints.
  header: Authorization
  how_to_obtain: Generate a team key in App Store Connect (Issuer ID, Key ID, and .p8 private key) and use Prisma to sign JWTs.
  location: header
  name: App Store Connect JWT
  type: jwt
slug: prismareviews-authentication
source_filename: prismareviews-authentication.yml
source_heading: Authentication Profile
source_url: https://prismareviews.com/docs/api-reference/authentication
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://prismareviews.com/docs/api-reference/authentication\nsources:\n- https://prismareviews.com/docs/api-reference/authentication\n- https://prismareviews.com/guides/app-store-connect-api-key-reviews\n- https://prismareviews.com/guides/trustpilot-api-key\n- https://prismareviews.com/guides/google-reviews-api-key\ndescription: Authentication methods described in the Prisma Reviews documentation\nschemes:\n- type: http-bearer\n  name: Prisma API Key\n  evidence: Every request to https://api.prismareviews.com/v1 needs an API key in the Authorization header, as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Get a live key and a test key from the Prisma dashboard after creating an account.\n- type: oauth2\n  name: Trustpilot OAuth2\n  evidence: 'Token requests authenticate with Authorization: Basic base64(API_KEY:API_SECRET) . For client credentials\
  \ ( grant docs ):'\n  location: header\n  header: Authorization\n  flows:\n  - client_credentials\n  token_url: https://api.trustpilot.com/v1/oauth/oauth-business-users-for-applications/accesstoken\n  how_to_obtain: Create an API application in Trustpilot Business to obtain the API key and secret, then request a token using the client_credentials\n    grant.\n- type: jwt\n  name: App Store Connect JWT\n  evidence: Every request to the App Store Connect API carries a JSON Web Token signed with the .p8 key (algorithm ES256), with the Key ID in\n    the header, the Issuer ID as iss and an expiry of at most 20 minutes for the reviews endpoints.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a team key in App Store Connect (Issuer ID, Key ID, and .p8 private key) and use Prisma to sign JWTs.\ndocs: https://prismareviews.com/docs/api-reference/authentication\n"
source_yaml_url: https://artifacts.apis.io/prismareviews/authentication/prismareviews-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Reviews
- Software-as-a-Service
- GDPR
- Spain
---
