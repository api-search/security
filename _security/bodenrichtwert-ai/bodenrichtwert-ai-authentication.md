---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods as documented
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: bodenrichtwert.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: bodenrichtwert.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: bodenrichtwert.ai
provider_slug: bodenrichtwert-ai
scheme_count: 2
schemes:
- evidence: 'Jeder Request braucht einen Token. Im Normalfall reist er im `Authorization: Bearer <token>`-Header — die einzige Ausnahme ist der Query-Parameter für Tabellen-Importer weiter unten.'
  header: Authorization
  how_to_obtain: Erstelle einen API‑Key im Dashboard → API‑Keys, erhalte den Token einmalig angezeigt.
  location: header
  name: API-Key
  type: http-bearer
- evidence: Client Credentials (M2M)
  header: Authorization
  how_to_obtain: Registriere eine vertrauliche OAuth‑App mit Grant‑Type `client_credentials` im Dashboard → OAuth‑Apps, dann erhalte ein Access‑Token via POST zu /oauth/token mit Basic‑Auth (client_id:client_secret).
  location: header
  name: Client Credentials
  token_url: https://bodenrichtwert.ai/oauth/token
  type: oauth2
slug: bodenrichtwert-ai-authentication
source_filename: bodenrichtwert-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://bodenrichtwert.ai/raw/docs/entwickler-einstieg/authentication.md
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://bodenrichtwert.ai/raw/docs/entwickler-einstieg/authentication.md\nsources:\n- https://bodenrichtwert.ai/raw/docs/entwickler-einstieg/authentication.md\n- https://bodenrichtwert.ai/raw/docs/entwickler-einstieg/oauth-app-registrieren.md\n- https://bodenrichtwert.ai/docs/integration-guides\n- https://bodenrichtwert.ai/docs/entwickler-einstieg/authentication\ndescription: Authentication methods as documented\nschemes:\n- type: http-bearer\n  name: API-Key\n  evidence: 'Jeder Request braucht einen Token. Im Normalfall reist er im `Authorization: Bearer <token>`-Header — die einzige Ausnahme ist der\n    Query-Parameter für Tabellen-Importer weiter unten.'\n  location: header\n  header: Authorization\n  how_to_obtain: Erstelle einen API‑Key im Dashboard → API‑Keys, erhalte den Token einmalig angezeigt.\n- type: oauth2\n  name: Client Credentials\n  evidence: Client Credentials\
  \ (M2M)\n  location: header\n  header: Authorization\n  token_url: https://bodenrichtwert.ai/oauth/token\n  how_to_obtain: Registriere eine vertrauliche OAuth‑App mit Grant‑Type `client_credentials` im Dashboard → OAuth‑Apps, dann erhalte ein Access‑Token\n    via POST zu /oauth/token mit Basic‑Auth (client_id:client_secret).\ndocs: https://bodenrichtwert.ai/raw/docs/entwickler-einstieg/authentication.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/bodenrichtwert-ai/authentication/bodenrichtwert-ai-authentication.yml
summary_line: 2 schemes
tags:
- Real Estate
- Artificial Intelligence
- Data API
- Germany
- Property Valuation
- Company
---
