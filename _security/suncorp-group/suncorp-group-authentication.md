---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Suncorp Group Authentication
name_suffix: Authentication
oauth_flows: []
overview: Suncorp Group declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Suncorp Group
provider_slug: suncorp-group
scheme_count: 0
schemes: []
slug: suncorp-group-authentication
source_filename: suncorp-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://www.vero.com.au/terms-sid.html, https://www.vero.com.au/broker/tools.html,\n  https://www.vero.com.au/secure/veroedge.html and live 2026-07-25 probes of\n  online.verocentral.com.au. No OpenAPI exists to derive from —\n  derive-authentication.py has no spec input for this provider.\npublic_api: false\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  machine_to_machine_auth_documented: false\n  reading: >-\n    There is no public API and therefore no public API authentication scheme. No\n    API keys, no client-credentials flow, no mTLS onboarding and no scope model\n    are documented anywhere on Suncorp Group or brand properties. The only access\n    model Suncorp publishes is a human, browser-based federated single sign-on to\n    gated broker portals, granted person-by-person by a Vero representative.\nschemes: []\ngated_access_model:\n- name: Access Single ID (SID)\n  kind: browser-federated-sso\n\
  \  audience: brokers and intermediaries\n  entry_point: https://www.vero.com.au/secure/veroedge.html\n  identity_provider: https://online.verocentral.com.au/idp/channel/vero-portal\n  identity_provider_status: 200\n  presentation: HTML login form titled \"Vero Intermediary Portal\"\n  terms: https://www.vero.com.au/terms-sid.html\n  provisioning: >-\n    Granted by a dedicated Vero Representative per the Vero broker tools page —\n    a human onboarding path, not self-serve registration.\n  discovery_documents:\n    openid_configuration: 404\n    oauth_authorization_server: 404\n  capabilities_behind_the_wall:\n  - SME Package and Commercial Motor quoting with real-time response\n  - New business bind and full policy lifecycle transactions\n  - Renewals including Workers Compensation\n  - Electronic document access (schedules, new business, renewals)\n- name: Engineers PI & Strata Portal (Uniwriter)\n  kind: third-party-underwriting-application\n  audience: brokers\n  entry_point: https://EngineersPIandStrataPortal.vero.com.au/\n\
  \  entry_point_status: 200\n  presentation: Angular single-page application\n  discovery_documents:\n    openid_configuration: >-\n      200 but serves the SPA HTML shell, not a discovery document — does not parse\n      as JSON\nmachine_channels:\n  note: >-\n    The primary machine-to-machine path is a Broker Management System connection\n    over Australia's commercial broker trading networks (Steadfast SCTP, Sunrise\n    Exchange). Credentials and message formats for those channels are commercial\n    and are not published by Suncorp — see\n    conformance/suncorp-group-conformance.yml.\n  publicly_documented: false\npointer_note: >-\n  Deliberately NOT wired as `type: Authentication` in apis.yml. That scoring check\n  reads \"API authentication is documented,\" and Suncorp Group documents no API\n  authentication — only a human portal login. Wiring the pointer would award\n  points for something that does not exist.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/suncorp-group/refs/heads/main/authentication/suncorp-group-authentication.yml
summary_line: 0 schemes
tags:
- Insurance
- Australia
- Property and Casualty
- General Insurance
- Carrier
- Personal Lines
- Commercial Lines
- Claims
- Underwriting
- Brokers
- Partner Gated
- New Zealand
---
