---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailbox-bot-api-openapi.json
  format: json
  label: mailbox.bot API API
  slug: mailbox-bot-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailbox-bot/openapi/_original/mailbox-bot-api-openapi.json
auth_types: []
description: Authentication for mailbox.bot is performed using a bearer token (API key) sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mailbox.bot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailbox.bot declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mailbox.bot
provider_slug: mailbox-bot
scheme_count: 1
schemes:
- evidence: 'After the human creates an agent API key, send it as:


    ```http

    Authorization: Bearer sk_agent_...

    ```'
  header: Authorization
  how_to_obtain: Human operator creates an agent API key via the mailbox.bot UI after completing onboarding, billing, and approval steps.
  location: header
  name: Bearer
  type: http-bearer
slug: mailbox-bot-authentication
source_filename: mailbox-bot-authentication.yml
source_heading: Authentication Profile
source_url: https://mailbox.bot/auth.md
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mailbox.bot/auth.md\nsources:\n- https://mailbox.bot/auth.md\ndescription: Authentication for mailbox.bot is performed using a bearer token (API key) sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'After the human creates an agent API key, send it as:\n\n\n    ```http\n\n    Authorization: Bearer sk_agent_...\n\n    ```'\n  location: header\n  header: Authorization\n  how_to_obtain: Human operator creates an agent API key via the mailbox.bot UI after completing onboarding, billing, and approval steps.\nnote: The page describes OAuth metadata discovery but does not provide concrete OAuth2 token or authorize URLs, flows, or scopes for client use,\n  so no oauth2 scheme is listed.\ndocs: https://mailbox.bot/auth.md\n"
source_yaml_url: https://artifacts.apis.io/mailbox-bot/authentication/mailbox-bot-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Mail
- Automation
- Postal
---
