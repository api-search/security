---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Infakt Authentication
name_suffix: Authentication
oauth_flows: []
overview: inFakt secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: inFakt
provider_slug: infakt
scheme_count: 1
schemes:
- description: Per-account API key generated in the inFakt web app. Sent on every request in the X-inFakt-ApiKey header. A missing key returns HTTP 401 with body {"error":"Musisz podac klucz API."}; an invalid key returns HTTP 401 with {"error":"Klucz API ktory podales jest nieprawidlowy."}. inFakt provides a separate Sandbox environment with its own test API key (see sandbox/).
  evidence:
  - GET https://api.infakt.pl/api/v3/clients.json without header -> 401 "Musisz podac klucz API."
  - GET .../clients.json with junk X-inFakt-ApiKey -> 401 "Klucz API ktory podales jest nieprawidlowy."
  in: header
  name: inFaktApiKey
  parameter_name: X-inFakt-ApiKey
  type: apiKey
slug: infakt-authentication
source_filename: infakt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.infakt.pl/ + live probe of https://api.infakt.pl/api/v3/\ndocs: https://docs.infakt.pl/\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: inFaktApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-inFakt-ApiKey\n  description: >-\n    Per-account API key generated in the inFakt web app. Sent on every request\n    in the X-inFakt-ApiKey header. A missing key returns HTTP 401 with body\n    {\"error\":\"Musisz podac klucz API.\"}; an invalid key returns HTTP 401 with\n    {\"error\":\"Klucz API ktory podales jest nieprawidlowy.\"}. inFakt provides a\n    separate Sandbox environment with its own test API key (see sandbox/).\n  evidence:\n  - 'GET https://api.infakt.pl/api/v3/clients.json without header -> 401 \"Musisz podac klucz API.\"'\n  - 'GET .../clients.json with junk X-inFakt-ApiKey -> 401 \"Klucz API ktory podales jest nieprawidlowy.\"'\nnotes: >-\n  Key-auth\
  \ only. inFakt does not expose OAuth2 or OpenID Connect\n  (/.well-known/openid-configuration and /oauth-authorization-server both 404),\n  so there is no OAuth scope surface for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infakt/refs/heads/main/authentication/infakt-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Accounting
- Invoicing
- Fintech
- Bookkeeping
- e-Invoicing
- KSeF
- Tax
- Poland
- SMB
---
