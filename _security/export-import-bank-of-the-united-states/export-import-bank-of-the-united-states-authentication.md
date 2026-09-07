---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Export Import Bank Of The United States Authentication
name_suffix: Authentication
oauth_flows: []
overview: Export-Import Bank of the United States declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Export-Import Bank of the United States
provider_slug: export-import-bank-of-the-united-states
scheme_count: 0
schemes: []
slug: export-import-bank-of-the-united-states-authentication
source_filename: export-import-bank-of-the-united-states-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live unauthenticated fetches of every EXIM surface, 2026-09-04\nsummary:\n  types: []\n  public_surfaces_require_no_credential: true\nschemes: []\nnote: >-\n  There is no API to authenticate to. Every publicly reachable EXIM data surface is served\n  anonymously over plain HTTPS GET with no key, token, or header of any kind; every\n  authenticated surface is a human web application with no documented programmatic entry\n  point.\n  This file REPLACES an X-App-Token apiKey profile derived from a fabricated Socrata\n  OpenAPI. That header belonged to a data.exim.gov instance decommissioned on 2023-09-14.\n  See _quarantine/NOTE.md.\nsurfaces:\n- surface: EXIM Open Data catalog (data.json + CSV + PDF)\n  host: img.exim.gov\n  auth: none\n  verified:\n    url: https://img.exim.gov/s3fs-public/dataset/vbhv-d8am/data.json\n    http_status: 200\n    sent_credentials: false\n- surface: EXIM Digital Archives (OCLC CONTENTdm / IIIF)\n\
  \  host: www.digitalarchives.exim.gov\n  auth: none\n  operator: vendor\n  operator_name: OCLC CONTENTdm\n  verified:\n    url: https://www.digitalarchives.exim.gov/digital/api/collections\n    http_status: 200\n    sent_credentials: false\n- surface: EXIM Online application portal\n  host: eximonline.exim.gov\n  auth: gated\n  auth_mechanism: unknown\n  note: >-\n    Interactive login for export-finance applicants, carrying a Controlled Unclassified\n    Information banner. No public developer documentation, no OAuth/OIDC discovery\n    document (/.well-known/openid-configuration returns the SPA shell, not metadata), and\n    no published API. The mechanism cannot be determined without an account, and this\n    pipeline does not create one.\n  verified:\n    url: https://eximonline.exim.gov/\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/export-import-bank-of-the-united-states/refs/heads/main/authentication/export-import-bank-of-the-united-states-authentication.yml
summary_line: 0 schemes
tags:
- Export
- Federal-Government
- Finance
- Import
- Open Data
- Trade Finance
---
