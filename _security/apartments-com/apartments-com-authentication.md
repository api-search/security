---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Apartments Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apartments.com declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Apartments.com
provider_slug: apartments-com
scheme_count: 0
schemes: []
slug: apartments-com-authentication
source_filename: apartments-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  https://propertyhelp.apartments.com/ (ILS + MLS integration collections),\n  live probes of every apartments.com host\napi_authentication: none published\npointer: >-\n  withheld — the ergonomics check `authentication_documented` asks whether a\n  developer-facing API documents how to authenticate. Apartments.com exposes\n  no such API, so no `Authentication` pointer is wired. This artifact records\n  the ONLY credential models that exist, both of which are partner seams.\nsummary:\n  types: []\n  api_key: false\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  developer_credentials_obtainable: false\nschemes: []\npartner_seams:\n- name: digital-feeds-ftp\n  direction: inbound (vendor -> Apartments.com)\n  mechanism: FTP username/password issued out-of-band\n  evidence: >-\n    https://propertyhelp.apartments.com/article/1041-how-do-i-connect-my-listing-to-apartmentscom-using-mri-market-connect\n    (HTTP\
  \ 200): \"Prerequisites — You must identify the following FTP server\n    information from the ILS you wish to add: FTP Server Name, FTP Login\n    (Username), FTP Password.\"\n  gate: >-\n    Requires (a) a paying Apartments.com advertising contract, (b) application\n    via Feeds@apartments.com or\n    https://www.apartments.com/advertise/advfeeds, and (c) an approved\n    third-party feed vendor. No API key is ever issued and no data returns to\n    the caller.\n- name: mls-syndication-optin\n  direction: inbound (MLS -> Apartments.com)\n  mechanism: >-\n    No credential is issued to the publisher at all — a licensed agent toggles\n    Apartments.com syndication inside their own MLS system.\n  evidence: https://propertyhelp.apartments.com/collection/1201-mls-integrations (HTTP 200)\n  gate: MLS membership (Bright MLS, ARMLS, REcolorado, OneKey MLS, SmartMLS,\n    NorthstarMLS, MLS PIN, Garden State MLS, New Jersey MLS, Aspen Glenwood MLS\n    documented) plus, in practice, a real-estate\
  \ licence.\n- name: web-session-login\n  direction: human\n  mechanism: ordinary web session login (no documented developer scheme)\n  urls:\n  - https://www.apartments.com/prosumer/login/\n  - https://www.apartments.com/customers/login\n  note: >-\n    Both return HTTP 403 to non-browser clients; they are account portals for\n    landlords and renters, not an identity provider a developer can integrate.\ndiscovery_probes:\n- {url: 'https://www.apartments.com/.well-known/openid-configuration', status: 403}\n- {url: 'https://api.apartments.com/.well-known/openid-configuration', status: 403}\n- {url: 'https://www.apartments.com/.well-known/oauth-authorization-server', status: 403}\n- {url: 'https://api.apartments.com/.well-known/oauth-authorization-server', status: 403}\n- {url: 'https://propertyhelp.apartments.com/.well-known/openid-configuration', status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apartments-com/refs/heads/main/authentication/apartments-com-authentication.yml
summary_line: 0 schemes
tags:
- Real Estate
- United States
- Rentals
- Property Listings
- Multifamily
- Internet Listing Service
- Listings Syndication
- Property Management
- MLS
- PropTech
- CoStar Group
---
