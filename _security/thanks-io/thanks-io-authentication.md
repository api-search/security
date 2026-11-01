---
anonymous_access: false
api_key_in: []
api_specs:
- filename: thanks-io-creatives-library-api-openapi.yml
  format: yaml
  label: Thanks.io Creatives Library API
  slug: thanks-io-creatives-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-creatives-library-api-openapi.yml
- filename: thanks-io-dynamic-images-api-openapi.yml
  format: yaml
  label: Thanks.io Dynamic Images API
  slug: thanks-io-dynamic-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-dynamic-images-api-openapi.yml
- filename: thanks-io-giftcards-api-openapi.yml
  format: yaml
  label: Thanks.io Giftcards API
  slug: thanks-io-giftcards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-giftcards-api-openapi.yml
- filename: thanks-io-handwriting-styles-api-openapi.yml
  format: yaml
  label: Thanks.io Handwriting Styles API
  slug: thanks-io-handwriting-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-handwriting-styles-api-openapi.yml
- filename: thanks-io-image-templates-api-openapi.yml
  format: yaml
  label: Thanks.io Image Templates API
  slug: thanks-io-image-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-image-templates-api-openapi.yml
- filename: thanks-io-mailing-lists-api-openapi.yml
  format: yaml
  label: Thanks.io Mailing Lists API
  slug: thanks-io-mailing-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-mailing-lists-api-openapi.yml
- filename: thanks-io-message-templates-api-openapi.yml
  format: yaml
  label: Thanks.io Message Templates API
  slug: thanks-io-message-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-message-templates-api-openapi.yml
- filename: thanks-io-order-estimates-api-openapi.yml
  format: yaml
  label: Thanks.io Order Estimates API
  slug: thanks-io-order-estimates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-order-estimates-api-openapi.yml
- filename: thanks-io-orders-api-openapi.yml
  format: yaml
  label: Thanks.io Orders API
  slug: thanks-io-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-orders-api-openapi.yml
- filename: thanks-io-recipients-api-openapi.yml
  format: yaml
  label: Thanks.io Recipients API
  slug: thanks-io-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-recipients-api-openapi.yml
- filename: thanks-io-send-mailer-api-openapi.yml
  format: yaml
  label: Thanks.io Send Mailer API
  slug: thanks-io-send-mailer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-send-mailer-api-openapi.yml
- filename: thanks-io-webhook-events-api-openapi.yml
  format: yaml
  label: Thanks.io Webhook Events API
  slug: thanks-io-webhook-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-webhook-events-api-openapi.yml
- filename: thanks-io-webhooks-api-openapi.yml
  format: yaml
  label: Thanks.io Webhooks API
  slug: thanks-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-webhooks-api-openapi.yml
- filename: thanks-io-subaccounts-api-openapi.yml
  format: yaml
  label: Thanks.io Subaccounts API
  slug: thanks-io-subaccounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thanks-io/openapi/thanks-io-subaccounts-api-openapi.yml
auth_types: []
description: Authentication methods for thanks.io API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Thanks Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thanks.io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Thanks.io
provider_slug: thanks-io
scheme_count: 2
schemes:
- evidence: All API requests must be authenticated with a bearer token. Create one in your dashboard under **Settings → [API Access](https://dashboard.thanks.io/app/settings/api-access)**
  header: Authorization
  how_to_obtain: Create a token in the dashboard under Settings → API Access → API Keys and copy it.
  location: header
  name: Bearer Token
  type: http-bearer
- authorize_url: https://dashboard.thanks.io/oauth/authorize?response_type=code&client_id=YOUR_CLIENT_ID&redirect_uri=YOUR_REDIRECT_URI
  evidence: Thanks.io supports OAuth 2.0 for secure authentication and authorization.
  header: Authorization
  how_to_obtain: Register an OAuth application in the dashboard under Settings → API Access to obtain a client ID and client secret.
  location: header
  name: OAuth
  token_url: https://dashboard.thanks.io/oauth/token
  type: oauth2
slug: thanks-io-authentication
source_filename: thanks-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.thanks.io/authentication/choosing-auth-method.md
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.thanks.io/authentication/choosing-auth-method.md\nsources:\n- https://docs.thanks.io/authentication/choosing-auth-method.md\n- https://docs.thanks.io/authentication/bearer-token.md\n- https://docs.thanks.io/authentication/oauth.md\n- https://help.thanks.io/api/generate-an-api-key/\ndescription: Authentication methods for thanks.io API\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: All API requests must be authenticated with a bearer token. Create one in your dashboard under **Settings → [API Access](https://dashboard.thanks.io/app/settings/api-access)**\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in the dashboard under Settings → API Access → API Keys and copy it.\n- type: oauth2\n  name: OAuth\n  evidence: Thanks.io supports OAuth 2.0 for secure authentication and authorization.\n  location: header\n  header: Authorization\n\
  \  token_url: https://dashboard.thanks.io/oauth/token\n  authorize_url: https://dashboard.thanks.io/oauth/authorize?response_type=code&client_id=YOUR_CLIENT_ID&redirect_uri=YOUR_REDIRECT_URI\n  how_to_obtain: Register an OAuth application in the dashboard under Settings → API Access to obtain a client ID and client secret.\nnote: No explicit scopes are listed in the documentation.\ndocs: https://docs.thanks.io/authentication/choosing-auth-method.md\n"
source_yaml_url: https://artifacts.apis.io/thanks-io/authentication/thanks-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- DirectMail
- Automation
- API
---
