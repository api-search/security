---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pocket-id-openapi-generated.yml
  format: yaml
  label: Pocket ID API
  slug: pocket-id-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pocket-id/openapi/_ae-authored/pocket-id-openapi-generated.yml
auth_types: []
description: Authentication schemes for Pocket ID
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Pocket Id Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pocket ID declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Pocket ID
provider_slug: pocket-id
scheme_count: 2
schemes:
- evidence: 'Send the key in the X-API-KEY header:'
  header: X-API-KEY
  how_to_obtain: Open Administration → API Keys and click Add API Key.
  location: header
  name: API Key
  type: apiKey
- evidence: 'Instead of client_secret , it sends these two parameters to the token endpoint: client_assertion_type=urn:ietf:params:oauth:client-assertion-type:jwt-bearer client_assertion=<token from the platform>'
  flows:
  - client_credentials
  how_to_obtain: Add Federated Client Credential in the client’s Credentials tab under Administration → OIDC Clients.
  location: body
  name: Federated client credentials
  type: oauth2
slug: pocket-id-authentication
source_filename: pocket-id-authentication.yml
source_heading: Authentication Profile
source_url: https://pocket-id.org/docs/guides/oidc-client-authentication
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://pocket-id.org/docs/guides/oidc-client-authentication\nsources:\n- https://pocket-id.org/docs/guides/oidc-client-authentication\n- https://pocket-id.org/docs/guides/proxy-services\n- https://pocket-id.org/docs/api\n- https://pocket-id.org/docs/advanced/custom-keys\ndescription: Authentication schemes for Pocket ID\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Send the key in the X-API-KEY header:'\n  location: header\n  header: X-API-KEY\n  how_to_obtain: Open Administration → API Keys and click Add API Key.\n- type: oauth2\n  name: Federated client credentials\n  evidence: 'Instead of client_secret , it sends these two parameters to the token endpoint: client_assertion_type=urn:ietf:params:oauth:client-assertion-type:jwt-bearer\n    client_assertion=<token from the platform>'\n  location: body\n  flows:\n  - client_credentials\n  how_to_obtain: Add Federated Client\
  \ Credential in the client’s Credentials tab under Administration → OIDC Clients.\ndocs: https://pocket-id.org/docs/guides/oidc-client-authentication\n"
source_yaml_url: https://artifacts.apis.io/pocket-id/authentication/pocket-id-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Identity
- OpenID Connect
- OAuth2
- Self-Hosted
---
