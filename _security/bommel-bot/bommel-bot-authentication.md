---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bommel-bot-agent-api-openapi.yml
  format: yaml
  label: bommel-bot Agent API
  slug: bommel-bot-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bommel-bot/openapi/bommel-bot-agent-api-openapi.yml
auth_types: []
description: Authentication methods described in Bommel Bot documentation
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bommel Bot Authentication
name_suffix: Authentication
oauth_flows: []
overview: bommel-bot declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: bommel-bot
provider_slug: bommel-bot
scheme_count: 2
schemes:
- evidence: It goes in your server settings only. It is never sent to the browser and never appears in a page's source.
  how_to_obtain: Create an API key at https://aistudio.google.com/apikey, copy it, and set it in your server environment variables.
  name: GEMINI_API_KEY
  type: apiKey
- evidence: The other three checkers use Bommel's "ID badge" — a Firebase service account.
  how_to_obtain: Generate a new private key for a Firebase service account in the Firebase console and set the environment variables FIREBASE_ADMIN_CLIENT_EMAIL, FIREBASE_ADMIN_PRIVATE_KEY, and FIREBASE_ADMIN_PROJECT_ID (or point GOOGLE_APPLICATION_CREDENTIALS to the JSON file).
  name: Firebase service account
  type: other
slug: bommel-bot-authentication
source_filename: bommel-bot-authentication.yml
source_heading: Authentication Profile
source_url: https://bommel.bot/help/quick-start
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://bommel.bot/help/quick-start\nsources:\n- https://bommel.bot/help/quick-start\n- https://bommel.bot/help/content-safety-apis-setup\ndescription: Authentication methods described in Bommel Bot documentation\nschemes:\n- type: apiKey\n  name: GEMINI_API_KEY\n  evidence: It goes in your server settings only. It is never sent to the browser and never appears in a page's source.\n  how_to_obtain: Create an API key at https://aistudio.google.com/apikey, copy it, and set it in your server environment variables.\n- type: other\n  name: Firebase service account\n  evidence: The other three checkers use Bommel's \"ID badge\" — a Firebase service account.\n  how_to_obtain: Generate a new private key for a Firebase service account in the Firebase console and set the environment variables FIREBASE_ADMIN_CLIENT_EMAIL,\n    FIREBASE_ADMIN_PRIVATE_KEY, and FIREBASE_ADMIN_PROJECT_ID (or point\
  \ GOOGLE_APPLICATION_CREDENTIALS to the JSON file).\ndocs: https://bommel.bot/help/quick-start\n"
source_yaml_url: https://artifacts.apis.io/bommel-bot/authentication/bommel-bot-authentication.yml
summary_line: 2 schemes
tags:
- Company
---
