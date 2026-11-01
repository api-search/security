---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Normi API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Normi Fr Authentication
name_suffix: Authentication
oauth_flows: []
overview: normi-fr declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: normi-fr
provider_slug: normi-fr
scheme_count: 3
schemes:
- evidence: 'X-API-Key: normi_abc123'
  header: X-API-Key
  how_to_obtain: Create a token in Dashboard → Tokens → Créer un token and use the displayed token as the X-API-Key header value.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Authorization: Bearer normi_abc123'
  header: Authorization
  how_to_obtain: Create a token in Dashboard → Tokens → Créer un token and use the displayed token as the Bearer token in the Authorization header.
  location: header
  name: Authorization
  type: http-bearer
- evidence: Le flux authorization code avec PKCE (S256) et le jeton de rafraîchissement.
  how_to_obtain: Paste https://mcp.normi.fr/mcp into the client, log in to Normi, and authorize the application; the client handles token renewal automatically.
  name: OAuth2 Authorization Code with PKCE
  type: oauth2
slug: normi-fr-authentication
source_filename: normi-fr-authentication.yml
source_heading: Authentication Profile
source_url: https://www.normi.fr/docs/install/claude-code
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.normi.fr/docs/install/claude-code\nsources:\n- https://www.normi.fr/docs/install/claude-code\n- https://www.normi.fr/docs/concepts/authentication\n- https://www.normi.fr/docs/quickstart\ndescription: Authentication methods for Normi API\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'X-API-Key: normi_abc123'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a token in Dashboard → Tokens → Créer un token and use the displayed token as the X-API-Key header value.\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authorization: Bearer normi_abc123'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in Dashboard → Tokens → Créer un token and use the displayed token as the Bearer token in the Authorization header.\n- type: oauth2\n  name: OAuth2 Authorization Code with PKCE\n  evidence: Le flux authorization code\
  \ avec PKCE (S256) et le jeton de rafraîchissement.\n  how_to_obtain: Paste https://mcp.normi.fr/mcp into the client, log in to Normi, and authorize the application; the client handles token renewal\n    automatically.\ndocs: https://www.normi.fr/docs/install/claude-code\n"
source_yaml_url: https://artifacts.apis.io/normi-fr/authentication/normi-fr-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Real Estate
- Data API
- French Market
- Property Transactions
---
