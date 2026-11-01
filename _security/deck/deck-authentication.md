---
anonymous_access: false
api_key_in: []
api_specs:
- filename: deck-connection-api-openapi.yml
  format: yaml
  label: Deck Connection API
  slug: deck-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deck/openapi/deck-connection-api-openapi.yml
- filename: deck-jobs-api-openapi.yml
  format: yaml
  label: Deck Jobs API
  slug: deck-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deck/openapi/deck-jobs-api-openapi.yml
- filename: deck-link-api-openapi.yml
  format: yaml
  label: Deck Link API
  slug: deck-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deck/openapi/deck-link-api-openapi.yml
auth_types: []
description: Deck authenticates to source websites using credential objects that specify an `auth_method` and associated fields such as username, password, and optional source‑specific fields.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Deck Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deck declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Deck
provider_slug: deck
scheme_count: 2
schemes:
- evidence: '`auth_method`: `username_password`'
  name: username_password
  type: other
- evidence: '`auth_method`: `source_fields`'
  name: source_fields
  type: other
slug: deck-authentication
source_filename: deck-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.deck.co/concepts/credentials.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.deck.co/concepts/credentials.md\nsources:\n- https://docs.deck.co/concepts/credentials.md\n- https://docs.deck.co/guides/building-auth-ui.md\n- https://docs.deck.co/guides/quickstart.md\ndescription: Deck authenticates to source websites using credential objects that specify an `auth_method` and associated fields such as username,\n  password, and optional source‑specific fields.\nschemes:\n- type: other\n  name: username_password\n  evidence: '`auth_method`: `username_password`'\n- type: other\n  name: source_fields\n  evidence: '`auth_method`: `source_fields`'\ndocs: https://docs.deck.co/concepts/credentials.md\nnote: 3 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/deck/authentication/deck-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Automation
- API Integration
- Enterprise
- Security
---
