---
api_key_in: []
auth_types:
- none
- mutualTLS
description: 'CAISO''s authentication posture is a clean two-tier split. The public data tier — the OASIS Download API at oasis.caiso.com/oasisapi and the Today''s Outlook CSV feeds at www.caiso.com/outlook — carries no authentication at all: no API key, no token, no account, no referrer check. This was verified by anonymous curl on 2026-07-27, which returned real zipped CSV market data. Everything else CAISO operates — market submission, dispatch, settlements, CMRI, SIBR, the WEM and RC portals — sits behind PKI client certificates issued to individuals sponsored by their company''s User Access Administrator (UAA), and CAISO states in writing that OASIS is the sole exception. A third, distinct gate covers the *documentation*: developer.caiso.com requires a signup reviewed against an ISO-recognized corporate email domain and a written justification, so the interface specification and API URL example documents are access-controlled even though the API they describe is not.'
kind: authentication
layout: security
method: searched
name: Caiso Authentication
name_suffix: Authentication
oauth_flows: []
overview: California ISO secures its APIs with none and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: California ISO
provider_slug: caiso
scheme_count: 2
schemes:
- applies_to:
  - CAISO OASIS Download API
  - CAISO Today's Outlook Data Feeds
  description: No credential of any kind. GET the servlet or the CSV path and the data is returned. Verified 2026-07-27 with SingleZip (SLD_FCST, HTTP 200, 8,952-byte zip) and with https://www.caiso.com/outlook/current/fuelsource.csv (HTTP 200, text/csv).
  name: anonymous
  required: false
  sources:
  - https://www.caiso.com/documents/oasis-frequently-asked-questions.pdf
  - live probe 2026-07-27
  type: none
- applies_to:
  - CAISO Market Participant Portal
  - CMRI / SIBR / settlements and other participant systems
  description: Digital certificate issued through CAISO to a named individual, requested and approved by that company's User Access Administrator. Not obtainable by the general public and not used by, or accepted on, the OASIS or Today's Outlook surfaces.
  name: caiso-pki-client-certificate
  required: true
  sources:
  - https://www.caiso.com/systems-applications/requesting-access-certificates
  - https://www.caiso.com/systems-applications/user-access-administrator-uaa
  type: mutualTLS
slug: caiso-authentication
source_filename: caiso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  CAISO published documentation plus anonymous live calls to the OASIS Download API and\n  the Today's Outlook feeds on 2026-07-27\ndocs: https://www.caiso.com/systems-applications/requesting-access-certificates\ndescription: >-\n  CAISO's authentication posture is a clean two-tier split. The public data tier — the\n  OASIS Download API at oasis.caiso.com/oasisapi and the Today's Outlook CSV feeds at\n  www.caiso.com/outlook — carries no authentication at all: no API key, no token, no\n  account, no referrer check. This was verified by anonymous curl on 2026-07-27, which\n  returned real zipped CSV market data. Everything else CAISO operates — market\n  submission, dispatch, settlements, CMRI, SIBR, the WEM and RC portals — sits behind\n  PKI client certificates issued to individuals sponsored by their company's User Access\n  Administrator (UAA), and CAISO states in writing that OASIS is the sole exception.\n  A third,\
  \ distinct gate covers the *documentation*: developer.caiso.com requires a\n  signup reviewed against an ISO-recognized corporate email domain and a written\n  justification, so the interface specification and API URL example documents are\n  access-controlled even though the API they describe is not.\nsummary:\n  types:\n  - none\n  - mutualTLS\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_public_tier: true\nschemes:\n- name: anonymous\n  type: none\n  applies_to:\n  - CAISO OASIS Download API\n  - CAISO Today's Outlook Data Feeds\n  required: false\n  description: >-\n    No credential of any kind. GET the servlet or the CSV path and the data is returned.\n    Verified 2026-07-27 with SingleZip (SLD_FCST, HTTP 200, 8,952-byte zip) and with\n    https://www.caiso.com/outlook/current/fuelsource.csv (HTTP 200, text/csv).\n  sources:\n  - https://www.caiso.com/documents/oasis-frequently-asked-questions.pdf\n  - live probe 2026-07-27\n- name: caiso-pki-client-certificate\n  type: mutualTLS\n\
  \  applies_to:\n  - CAISO Market Participant Portal\n  - CMRI / SIBR / settlements and other participant systems\n  required: true\n  description: >-\n    Digital certificate issued through CAISO to a named individual, requested and\n    approved by that company's User Access Administrator. Not obtainable by the general\n    public and not used by, or accepted on, the OASIS or Today's Outlook surfaces.\n  sources:\n  - https://www.caiso.com/systems-applications/requesting-access-certificates\n  - https://www.caiso.com/systems-applications/user-access-administrator-uaa\nregistration:\n  required_for_api: false\n  required_for_docs: true\n  docs_signup: https://developer.caiso.com/_login/developersignup.aspx\n  cost: free\n  notes: >-\n    OASIS FAQ Question One: \"Developer Site access requires Users to sign up with an ISO\n    recognized @domain email address and a detailed justification\" — free-mail domains\n    (gmail, yahoo, hotmail) are subject to rejection. No such gate exists on\
  \ the API\n    itself.\nnot_present:\n- oauth2\n- openIdConnect\n- apiKey\n- http-bearer\n- http-basic\ntransport_security:\n  https: true\n  note: >-\n    http:// requests to oasis.caiso.com 302-redirect to https:// at the BigIP edge. See\n    security/caiso-domain-security.yml — oasis.caiso.com negotiates TLS 1.2 and neither\n    host sets HSTS.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caiso/refs/heads/main/authentication/caiso-authentication.yml
summary_line: none/mutualTLS · 2 schemes
tags:
- Energy
- United States
- Electricity
- Energy Markets
- Grid
- Renewables
- System Operator
- Market Data
- California
---
