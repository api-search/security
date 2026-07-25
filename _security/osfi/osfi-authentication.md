---
api_key_in: []
auth_types:
- none
- portal-login
description: 'OSFI runs two entirely separate surfaces with two different auth models: an anonymous READ surface (its data on Canada''s Open Government Portal) and a gated WRITE/FILING surface (the Regulatory Reporting System behind Bank of Canada Connect).'
kind: authentication
layout: security
method: searched
name: Osfi Authentication
name_suffix: Authentication
oauth_flows: []
overview: OSFI secures its APIs with none and portal-login across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OSFI
provider_slug: osfi
scheme_count: 2
schemes:
- base_url: https://open.canada.ca/data/en/api/3/action
  detail: 'No API key, no token, no registration, no referer restriction. Every action in conventions/osfi-conventions.yml returned 200 unauthenticated. CKAN supports an Authorization: <api-token> header for authenticated actions, but none of the OSFI read actions need it.'
  name: anonymous
  sources:
  - live probe 2026-07-25
  surface: public data — CKAN 3 Action API over OSFI's Open Government datasets
  type: none
  verified: true
- detail: Human login only. Accounts are provisioned by a Local Registration Authority at the filing institution. No developer-facing auth documentation, no client-credentials flow, no mTLS profile, no published token endpoint.
  http_status: 401
  name: bank-of-canada-connect
  programmatic: false
  surface: regulatory filing — Regulatory Reporting System (RRS)
  type: portal-login
  url: https://connect-connexion.bank-banque-canada.ca/igw/apps/ami/portal/login
  verified: true
slug: osfi-authentication
source_filename: osfi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: live probes of https://open.canada.ca/data/en/api/3/action and https://connect-connexion.bank-banque-canada.ca\n  on 2026-07-25; https://www.osfi-bsif.gc.ca/en/data-forms/open-government-osfi-financial-data\ndescription: 'OSFI runs two entirely separate surfaces with two different auth models: an anonymous READ\n  surface (its data on Canada''s Open Government Portal) and a gated WRITE/FILING surface (the Regulatory\n  Reporting System behind Bank of Canada Connect).'\nsummary:\n  types:\n  - none\n  - portal-login\n  api_key_in: []\n  oauth2_flows: []\n  public_read_requires_credentials: false\nschemes:\n- name: anonymous\n  type: none\n  surface: public data — CKAN 3 Action API over OSFI's Open Government datasets\n  base_url: https://open.canada.ca/data/en/api/3/action\n  sources:\n  - live probe 2026-07-25\n  detail: 'No API key, no token, no registration, no referer restriction. Every action in conventions/osfi-conventions.yml\n\
  \    returned 200 unauthenticated. CKAN supports an Authorization: <api-token> header for authenticated\n    actions, but none of the OSFI read actions need it.'\n  verified: true\n- name: bank-of-canada-connect\n  type: portal-login\n  surface: regulatory filing — Regulatory Reporting System (RRS)\n  url: https://connect-connexion.bank-banque-canada.ca/igw/apps/ami/portal/login\n  http_status: 401\n  detail: Human login only. Accounts are provisioned by a Local Registration Authority at the filing institution.\n    No developer-facing auth documentation, no client-credentials flow, no mTLS profile, no published\n    token endpoint.\n  programmatic: false\n  verified: true\nwell_known:\n  openid_configuration:\n    url: https://www.osfi-bsif.gc.ca/.well-known/openid-configuration\n    status: 404\n  oauth_authorization_server:\n    url: https://open.canada.ca/.well-known/oauth-authorization-server\n    status: 404\n  note: No OIDC or OAuth discovery document is published on any OSFI or\
  \ portal host.\ndocs: https://www.osfi-bsif.gc.ca/en/data-forms/open-government-osfi-financial-data\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osfi/refs/heads/main/authentication/osfi-authentication.yml
summary_line: none/portal-login · 2 schemes
tags:
- Insurance
- Canada
- Regulator
- Life Insurance
- Property and Casualty
- Financial Regulation
- Prudential Supervision
- Open Data
- Risk Data
- Market Infrastructure
- Banking
- Basel III
- Capital Adequacy
- Regulatory Reporting
- Pensions
---
