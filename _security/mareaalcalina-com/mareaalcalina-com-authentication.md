---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mareaalcalina-com-me-api-openapi.yml
  format: yaml
  label: Marea Alcalina Me API
  slug: mareaalcalina-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mareaalcalina-com/openapi/mareaalcalina-com-me-api-openapi.yml
- filename: mareaalcalina-com-storefronts-api-openapi.yml
  format: yaml
  label: Marea Alcalina Storefronts API
  slug: mareaalcalina-com-storefronts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mareaalcalina-com/openapi/mareaalcalina-com-storefronts-api-openapi.yml
- filename: mareaalcalina-com-users-api-openapi.yml
  format: yaml
  label: Marea Alcalina Users API
  slug: mareaalcalina-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mareaalcalina-com/openapi/mareaalcalina-com-users-api-openapi.yml
- filename: mareaalcalina-com-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Marea Alcalina Webhook Endpoints API
  slug: mareaalcalina-com-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mareaalcalina-com/openapi/mareaalcalina-com-webhook-endpoints-api-openapi.yml
auth_types: []
description: Authentication for Marea Alcalina APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Marea Alcalina Authentication
name_suffix: Authentication
oauth_flows: []
overview: Marea Alcalina declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Marea Alcalina
provider_slug: mareaalcalina-com
scheme_count: 2
schemes:
- evidence: 'Pass the key in `Authorization: Bearer <key>` (preferred). `X-API-Key: <key>` is accepted as a fallback.'
  header: Authorization
  how_to_obtain: Mint a `mk_user_*` or `mk_dev_*` key from the developer/dashboard UI or receive it in the `POST /v1/users` response when bootstrapping a user.
  location: header
  name: Bearer
  type: http-bearer
- evidence: '`X-API-Key: <key>` is accepted as a fallback.'
  header: X-API-Key
  how_to_obtain: Mint a `mk_user_*` or `mk_dev_*` key from the developer/dashboard UI or receive it in the `POST /v1/users` response when bootstrapping a user.
  location: header
  name: X-API-Key
  type: apiKey
slug: mareaalcalina-com-authentication
source_filename: mareaalcalina-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.mareaalcalina.com/concepts/keys.md
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.mareaalcalina.com/concepts/keys.md\nsources:\n- https://docs.mareaalcalina.com/concepts/keys.md\n- https://docs.mareaalcalina.com/api/use-this-when-you-want-to-rotate-the-signing-secret-of-a-webhook-endpoint-returns-the-new-secret-once;-the-old-secret-stops-working-immediately\n- https://docs.mareaalcalina.com/quickstart/products.md\n- https://docs.mareaalcalina.com/quickstart/publish.md\ndescription: Authentication for Marea Alcalina APIs\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Pass the key in `Authorization: Bearer <key>` (preferred). `X-API-Key: <key>` is accepted as a fallback.'\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a `mk_user_*` or `mk_dev_*` key from the developer/dashboard UI or receive it in the `POST /v1/users` response when bootstrapping\n    a user.\n- type: apiKey\n  name: X-API-Key\n  evidence: '`X-API-Key:\
  \ <key>` is accepted as a fallback.'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Mint a `mk_user_*` or `mk_dev_*` key from the developer/dashboard UI or receive it in the `POST /v1/users` response when bootstrapping\n    a user.\nnote: No OAuth2 flows are documented for this provider.\ndocs: https://docs.mareaalcalina.com/concepts/keys.md\n"
source_yaml_url: https://artifacts.apis.io/mareaalcalina-com/authentication/mareaalcalina-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
