---
api_key_in: []
auth_types:
- none
- session
description: ''
kind: authentication
layout: security
method: searched
name: Gigacatalyst Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gigacatalyst secures its APIs with none and session across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gigacatalyst
provider_slug: gigacatalyst
scheme_count: 2
schemes:
- abuse_controls_documented:
  - 'Returning `password` is suppressed when the submitted email already has an account (`isNewWorkspace: false`), specifically to prevent account takeover by anyone who knows the address.'
  - Request payload capped at 500 KB.
  - Rejection rules on provider/operation/path/baseUrl shape (see conventions/).
  applies_to: POST https://v2.gigacatalyst.com/api/self-serve/register
  description: 'The self-serve registration endpoint accepts an anonymous POST. No API key, bearer token, OAuth flow, or signature is required or documented. Verified live on 2026-08-14: OPTIONS returns 204 with `allow: OPTIONS, POST`; GET returns 405.'
  name: none
  sources:
  - https://v2.gigacatalyst.com/agent.md
  type: none
- applies_to: https://v2.gigacatalyst.com (workspace UI)
  credential_handling_published: 'Both signInUrl and password are declared secrets by the provider: print once to the human, never write to a file, commit message, .env, note, or the agent''s transcript; tell the human to store the password in a password manager and change it after sign-in.'
  description: The workspace itself is email + password. Registration returns a single-use, short-lived `signInUrl` plus a permanent generated password so the human can sign in normally after the link expires. Sign-in at https://v2.gigacatalyst.com/login asks for email and password.
  name: session
  sources:
  - https://v2.gigacatalyst.com/agent.md
  type: session
slug: gigacatalyst-authentication
source_filename: gigacatalyst-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  https://v2.gigacatalyst.com/agent.md (provider-published API reference) and\n  https://gigacatalyst.com/trust\ndocs: https://v2.gigacatalyst.com/agent.md\nnote: >-\n  derive-authentication.py was not run because there is no OpenAPI in this repo to derive\n  from - Gigacatalyst publishes no machine-readable spec. This profile is read from the\n  provider's own published agent instructions and trust center, which document the auth\n  model in prose. Two distinct auth surfaces exist and are easy to conflate; they are\n  separated below.\nsummary:\n  types: [none, session]\n  api_key_in: []\n  oauth2_flows: []\n  headline: >-\n    Gigacatalyst's own public API operation is UNAUTHENTICATED by design. The provider says\n    so explicitly and explains the consequence: \"this endpoint is public, and handing back a\n    password for an existing address would let anyone who knows it take that account over.\"\nschemes:\n- name:\
  \ none\n  type: none\n  applies_to: POST https://v2.gigacatalyst.com/api/self-serve/register\n  description: >-\n    The self-serve registration endpoint accepts an anonymous POST. No API key, bearer token,\n    OAuth flow, or signature is required or documented. Verified live on 2026-08-14: OPTIONS\n    returns 204 with `allow: OPTIONS, POST`; GET returns 405.\n  sources: [https://v2.gigacatalyst.com/agent.md]\n  abuse_controls_documented:\n  - >-\n    Returning `password` is suppressed when the submitted email already has an account\n    (`isNewWorkspace: false`), specifically to prevent account takeover by anyone who knows\n    the address.\n  - Request payload capped at 500 KB.\n  - Rejection rules on provider/operation/path/baseUrl shape (see conventions/).\n- name: session\n  type: session\n  applies_to: https://v2.gigacatalyst.com (workspace UI)\n  description: >-\n    The workspace itself is email + password. Registration returns a single-use, short-lived\n    `signInUrl` plus\
  \ a permanent generated password so the human can sign in normally after\n    the link expires. Sign-in at https://v2.gigacatalyst.com/login asks for email and\n    password.\n  credential_handling_published: >-\n    Both signInUrl and password are declared secrets by the provider: print once to the\n    human, never write to a file, commit message, .env, note, or the agent's transcript;\n    tell the human to store the password in a password manager and change it after sign-in.\n  sources: [https://v2.gigacatalyst.com/agent.md]\ndownstream_credential_model:\n  note: >-\n    SEPARATE SURFACE - do not read these as Gigacatalyst's own auth. This is the vocabulary\n    Gigacatalyst uses to describe how the CUSTOMER's API is authenticated when it is\n    registered as an integration. It is a real published enum and useful signal about what\n    the platform can connect to, but it authenticates the customer's API, not Gigacatalyst's.\n  field: integrations[].authentication\n  default: bearer\n\
  \  values:\n  - value: none\n    note: >-\n      \"A connection declared `none` is switched on at signup: their apps read real data from\n      the first minute, with no credential step and no sample data.\"\n  - value: bearer\n  - value: token\n  - value: api_key_header\n    note: paired with `headerName` when the API expects a named header\n  - value: basic\n    note: credential form asks for two fields\n  - value: login_session\n    note: credential form asks for two fields\n  credential_documentation_requirement: >-\n    The agent is required to attach one `documents[]` entry of kind `authentication` per\n    integration that needs a credential, recording the scheme, the header, the NAME of the\n    environment variable the project reads it from, and where a new key is issued - never the\n    value, and never by opening the file that holds it.\n  runtime_model: >-\n    Per the trust center, generated apps run in the customer's environment \"using the same\n    credentials and permissions\
  \ as your logged-in user\" - Gigacatalyst does not hold a\n    separate admin connection to the customer's database or APIs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigacatalyst/refs/heads/main/authentication/gigacatalyst-authentication.yml
summary_line: none/session · 2 schemes
tags:
- Company
- Artificial Intelligence
- Software-as-a-Service
- Sales Enablement
- Solutions Engineering
- Customer Success
- Automation
- No-Code
- Agents
- Embedded Analytics
- Low-Code
- Developer Tools
- Y Combinator
---
