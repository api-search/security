---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aidoo-ai-openapi-generated.yml
  format: yaml
  label: Aidoo API
  slug: aidoo-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aidoo-ai/openapi/_ae-authored/aidoo-ai-openapi-generated.yml
auth_types: []
description: Authentication is performed via OAuth 2.1; you connect to Aidoo from Claude and authorize access in one click.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aidoo Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aidoo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Aidoo
provider_slug: aidoo-ai
scheme_count: 1
schemes:
- evidence: 'L''authentification se fait via OAuth 2.1 : vous vous connectez à Aidoo depuis Claude, puis vous autorisez l''accès en un clic.'
  flows:
  - authorization_code
  how_to_obtain: User logs in to Aidoo, selects workspace, and clicks "Autoriser" to grant access.
  name: OAuth 2.1
  type: oauth2
slug: aidoo-ai-authentication
source_filename: aidoo-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://aidoo.ai/fr/docs/connexion-claude
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://aidoo.ai/fr/docs/connexion-claude\nsources:\n- https://aidoo.ai/fr/docs/connexion-claude\ndescription: Authentication is performed via OAuth 2.1; you connect to Aidoo from Claude and authorize access in one click.\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: 'L''authentification se fait via OAuth 2.1 : vous vous connectez à Aidoo depuis Claude, puis vous autorisez l''accès en un clic.'\n  flows:\n  - authorization_code\n  how_to_obtain: User logs in to Aidoo, selects workspace, and clicks \"Autoriser\" to grant access.\ndocs: https://aidoo.ai/fr/docs/connexion-claude\n"
source_yaml_url: https://artifacts.apis.io/aidoo-ai/authentication/aidoo-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- ERP
- Odoo
- Automation
- French
---
