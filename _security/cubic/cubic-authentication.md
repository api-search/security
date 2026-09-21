---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cubic-umo-iq-public-feed-openapi.yml
  format: yaml
  label: Umo IQ Public Feed API
  slug: umo-iq-public-feed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cubic/refs/heads/main/openapi/cubic-umo-iq-public-feed-openapi.yml
auth_types: []
description: 'Authentication posture for the one Cubic API with public documentation. The Umo IQ Public Feed requires no credential of any kind — no key, no token, no header, no signed request. Access control is contractual rather than technical: the feed''s licence grants use to Umo IQ customer agencies and reserves the right to terminate or limit access, but the endpoint itself is open to anonymous callers and enforces only per-IP volume limits.'
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Cubic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cubic Corporation declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Cubic Corporation
provider_slug: cubic
scheme_count: 0
schemes: []
slug: cubic-authentication
source_filename: cubic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: https://retro.umoiq.com/xmlFeedDocs/NextBusXMLFeed.pdf\nprovider: Cubic Corporation\nproviderId: cubic\ndescription: >-\n  Authentication posture for the one Cubic API with public documentation. The Umo IQ Public\n  Feed requires no credential of any kind — no key, no token, no header, no signed request.\n  Access control is contractual rather than technical: the feed's licence grants use to Umo IQ\n  customer agencies and reserves the right to terminate or limit access, but the endpoint itself\n  is open to anonymous callers and enforces only per-IP volume limits.\napis:\n  - name: Umo IQ Public Feed API\n    baseURL: https://retro.umoiq.com/service\n    scheme: none\n    anonymous: true\n    schemes: []\n    note: >-\n      Confirmed 2026-09-19: nine commands were called on both /publicXMLFeed and /publicJSONFeed\n      with no Authorization header and no API key, and all nine returned data (HTTP 200). No\n      WWW-Authenticate\
  \ challenge, no 401, no key-issuance flow is documented in the PDF.\n    x-evidence:\n      verified: '2026-09-19'\n      probe: 'GET https://retro.umoiq.com/service/publicJSONFeed?command=agencyList'\n      status: 200\n      auth_headers_sent: none\noauth2: false\nopenIdConnect: false\nmutualTLS: false\napiKey: false\ngated_surfaces:\n  - name: Umo IQ agency portal\n    url: https://rider.umoiq.com/\n    note: >-\n      Agency-facing portal behind a login; the Umo IQ Portal User Guide is published as a PDF but\n      no machine-readable contract or public auth documentation was found.\n  - name: GRIDSMART API\n    url: https://support.gridsmart.com/support/solutions/articles/69000340533-gridsmart-api\n    note: >-\n      Documented on Cubic's Freshdesk support portal; probed 2026-09-19 and 302s to\n      https://support.gridsmart.com/support/login, so the auth model is not publicly readable.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cubic/refs/heads/main/authentication/cubic-authentication.yml
summary_line: 0 schemes
tags:
- Defense
- Transportation
- Technology
- Public Transit
- Fare Collection
- Real-Time Data
- Vehicle Location
- Intelligent Transportation Systems
---
