---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apizr-best-practices-openapi-generated.yml
  format: yaml
  label: APIZR best practices API
  slug: best-practices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apizr/refs/heads/main/openapi/_ae-authored/apizr-best-practices-openapi-generated.yml
- filename: apizr-core-openapi-generated.yml
  format: yaml
  label: APIZR core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apizr/refs/heads/main/openapi/_ae-authored/apizr-core-openapi-generated.yml
- filename: apizr-triggers-openapi-generated.yml
  format: yaml
  label: APIZR triggers API
  slug: triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apizr/refs/heads/main/openapi/_ae-authored/apizr-triggers-openapi-generated.yml
auth_types: []
description: Authentication methods supported by APIZR Ecosystem
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Apizr Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIZR declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: APIZR
provider_slug: apizr
scheme_count: 4
schemes:
- evidence: 'Ecosystem ajoute automatiquement l''en-tête `Authorization: Basic xxx`.'
  header: Authorization
  how_to_obtain: Provide a username and password in the authentication method configuration.
  location: header
  name: Basic Auth
  type: http-basic
- evidence: Ecosystem obtient le token et le rafraîchit automatiquement à expiration.
  how_to_obtain: Provide client ID, client secret and token URL (and optional scopes) in the authentication method configuration.
  name: OAuth 2
  type: oauth2
- evidence: Ecosystem injecte automatiquement ces valeurs lorsque la méthode est sélectionnée dans un nœud Requête HTTP(S), Agent ou Code.
  how_to_obtain: Provide key/value pairs for headers and/or query parameters in the authentication method configuration.
  location: header_or_query
  name: API Key
  type: apiKey
- evidence: Exécute un **code personnalisé** qui gère un token et sa date d'expiration.
  how_to_obtain: Provide custom JavaScript code that returns an accessToken and expiresIn, and specify where (header, query param, or cookie) and the name to inject.
  location: header_or_query_or_cookie
  name: Custom
  type: other
slug: apizr-authentication
source_filename: apizr-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ecosystem.apizr.io/en/docs/credentials/introduction/
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ecosystem.apizr.io/en/docs/credentials/introduction/\nsources:\n- https://docs.ecosystem.apizr.io/en/docs/credentials/introduction/\n- https://docs.ecosystem.apizr.io/docs/credentials/create-credential.md\n- https://docs.ecosystem.apizr.io/docs/credentials/use-in-workflows.md\n- https://docs.ecosystem.apizr.io/docs/credentials/types.md\ndescription: Authentication methods supported by APIZR Ecosystem\nschemes:\n- type: http-basic\n  name: Basic Auth\n  evidence: 'Ecosystem ajoute automatiquement l''en-tête `Authorization: Basic xxx`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Provide a username and password in the authentication method configuration.\n- type: oauth2\n  name: OAuth 2\n  evidence: Ecosystem obtient le token et le rafraîchit automatiquement à expiration.\n  how_to_obtain: Provide client ID, client secret and token URL (and optional\
  \ scopes) in the authentication method configuration.\n- type: apiKey\n  name: API Key\n  evidence: Ecosystem injecte automatiquement ces valeurs lorsque la méthode est sélectionnée dans un nœud Requête HTTP(S), Agent ou Code.\n  location: header_or_query\n  how_to_obtain: Provide key/value pairs for headers and/or query parameters in the authentication method configuration.\n- type: other\n  name: Custom\n  evidence: Exécute un **code personnalisé** qui gère un token et sa date d'expiration.\n  location: header_or_query_or_cookie\n  how_to_obtain: Provide custom JavaScript code that returns an accessToken and expiresIn, and specify where (header, query param, or cookie)\n    and the name to inject.\ndocs: https://docs.ecosystem.apizr.io/en/docs/credentials/introduction/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apizr/refs/heads/main/authentication/apizr-authentication.yml
summary_line: 4 schemes
tags:
- iPaaS
- AI
- Integration
- Automation
- French
---
