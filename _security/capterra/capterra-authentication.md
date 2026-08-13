---
api_key_in: []
auth_types: []
description: Authentication profile for the Capterra Click Report API. Capterra publishes no OpenAPI and no public authentication reference — the API documentation lives inside the vendor console behind a login (PPC Bidding -> API Documentation), so this profile is built from a live unauthenticated probe of the API host plus the publicly stated credential-issuance process. Nothing here is inferred from a specification, because there is none to read.
kind: authentication
layout: security
method: probed
name: Capterra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capterra declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Capterra
provider_slug: capterra
scheme_count: 0
schemes: []
slug: capterra-authentication
source_filename: capterra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://public-api.capterra.com/v1/clicks (live unauthenticated probe,\n  2026-08-12) plus the publicly documented credential-issuance path\ndescription: >-\n  Authentication profile for the Capterra Click Report API. Capterra publishes no\n  OpenAPI and no public authentication reference — the API documentation lives\n  inside the vendor console behind a login (PPC Bidding -> API Documentation), so\n  this profile is built from a live unauthenticated probe of the API host plus the\n  publicly stated credential-issuance process. Nothing here is inferred from a\n  specification, because there is none to read.\nprovider: Capterra\nproviderId: capterra\napis:\n  - name: Capterra Click Report API\n    base_url: https://public-api.capterra.com/v1\n    schemes:\n      - id: api_key\n        type: apiKey\n        name: api_key\n        confirmed: true\n        transport: unverified\n        note: >-\n          The credential is\
  \ a vendor-issued API key. The parameter name `api_key`\n          is the name Capterra's own gated Swagger console uses (per the\n          \"Authorize\" flow described by integration partners), but the transport —\n          query parameter vs. header — could NOT be verified anonymously: a request\n          carrying a syntactically well-formed but invalid value in `?api_key=`\n          returns exactly the same 401 body as a request with no credential at all,\n          so the probe cannot distinguish \"rejected key\" from \"no key\". Recorded as\n          unverified rather than guessed.\n    issuance:\n      self_service: false\n      method: account-manager\n      note: >-\n        API keys are not self-service. A vendor must be enrolled in the\n        Capterra / G2 Digital Markets pay-per-click program and request the key\n        from their assigned account manager; the contact is surfaced inside the\n        vendor console under PPC Bidding -> API Documentation.\n      documented_at:\
  \ vendor console (login required)\n    oauth2: false\n    openid_connect: false\n    mutual_tls: false\n    scopes: none\n    scope_note: >-\n      Key authentication only — there is no OAuth surface, therefore no scope\n      model. A key is bound to a vendor and returns data for every Gartner Digital\n      Markets / G2 Digital Markets account mapped to that vendor (Capterra, GetApp,\n      Software Advice).\nevidence:\n  - url: https://public-api.capterra.com/v1/clicks\n    method: GET\n    http_status: 401\n    content_type: application/json; charset=utf-8\n    body: '{\"error\":\"Unauthorized\"}'\n    fetched: '2026-08-12'\n    note: >-\n      Live, first-party API host on capterra.com. The 401 is the proof the endpoint\n      exists and is credential-gated; sibling paths (/v1/click-report,\n      /v1/reports/clicks, /v1/health) return 404, and POST to /v1/clicks returns\n      404, so GET is the only routed method on this path.\n  - url: https://public-api.capterra.com/v1/clicks?api_key=REDACTED_TEST\n\
  \    method: GET\n    http_status: 401\n    fetched: '2026-08-12'\n    note: Invalid credential returns the same envelope; transport not distinguishable.\n  - url: https://www.capterra.com/vp/login\n    http_status: 404\n    fetched: '2026-08-12'\n    note: >-\n      The historically documented vendor-portal login — the door to the API\n      documentation — now 404s. Vendor login moved to\n      https://app.g2digitalmarkets.com/ after G2 acquired Capterra from Gartner\n      (closed 2026-02-05).\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capterra/refs/heads/main/authentication/capterra-authentication.yml
summary_line: 0 schemes
tags:
- Advertising
- B2B
- Click Reporting
- G2 Digital Markets
- Gartner Digital Markets
- Lead Generation
- Marketplace
- PPC
- Software Advice
- Software Comparison
- Software Reviews
---
