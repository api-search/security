---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Audigent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Audigent declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Audigent
provider_slug: audigent
scheme_count: 2
schemes:
- applies_to:
  - https://id.hadron.ad.gt/api/v1/pbhid
  - https://seg.hadron.ad.gt/api/v1/rtd
  - https://analytics.hadron.ad.gt/api/v1/analytics
  - https://cdn.hadronid.net/hadron.js
  description: Numeric Audigent Partner ID, issued by Audigent to a publisher or partner during onboarding and passed as a query parameter. The Prebid docs call it required for the RTD module ("This is the Audigent Partner ID obtained from Audigent"), but it is a tenant identifier embedded in client-side page JavaScript, not a secret — it is visible to anyone viewing the page source.
  id: partner_id
  in: query
  name: partner_id
  secret: false
  type: identifier
  x-evidence:
    fetched: '2026-08-06'
    http_status: 200
    note: Returned application/json with a freshly minted hadronId for an anonymous caller with partner_id=0 and no credential of any kind. Response values are per-browser identifiers and are deliberately not recorded here.
    url: https://id.hadron.ad.gt/api/v1/pbhid?partner_id=0&_it=prebid&t=1&src=id&domain=example.com
- applies_to:
  - https://api.audigent.com
  - https://admin.audigent.com
  description: 'Customer/partner console login. The API host runs gunicorn behind a Django stack and issues a 302 to https://admin.audigent.com for anonymous requests; response headers advertise session cookie handling (Vary: Origin, Cookie), X-Frame-Options DENY and Cross-Origin-Opener-Policy same-origin. No public sign-up, no documented token endpoint, no OAuth metadata.'
  id: console_session
  in: cookie
  secret: true
  type: session
  x-evidence:
    fetched: '2026-08-06'
    http_status: 302
    location: https://admin.audigent.com
    url: https://api.audigent.com/
slug: audigent-authentication
source_filename: audigent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: >-\n  https://docs.prebid.org/dev-docs/modules/hadronRtdProvider.html ;\n  https://github.com/prebid/Prebid.js/blob/master/modules/hadronIdSystem.js ;\n  live anonymous probes of id.hadron.ad.gt / seg.hadron.ad.gt / api.audigent.com\n\nsummary: >-\n  Audigent publishes no OpenAPI and no developer auth reference. Its public\n  ad-tech endpoints are unauthenticated by design — they are browser-side\n  identity and segment calls that carry a non-secret numeric partner_id rather\n  than a credential. The authenticated surface is the platform console at\n  admin.audigent.com, whose API host 302s every anonymous request to a login.\n  There is no API-key issuance page, no OAuth surface, and no documented token.\n\nschemes:\n- id: partner_id\n  type: identifier\n  in: query\n  name: partner_id\n  secret: false\n  applies_to:\n  - https://id.hadron.ad.gt/api/v1/pbhid\n  - https://seg.hadron.ad.gt/api/v1/rtd\n  - https://analytics.hadron.ad.gt/api/v1/analytics\n\
  \  - https://cdn.hadronid.net/hadron.js\n  description: >-\n    Numeric Audigent Partner ID, issued by Audigent to a publisher or partner\n    during onboarding and passed as a query parameter. The Prebid docs call it\n    required for the RTD module (\"This is the Audigent Partner ID obtained from\n    Audigent\"), but it is a tenant identifier embedded in client-side page\n    JavaScript, not a secret — it is visible to anyone viewing the page source.\n  x-evidence:\n    fetched: '2026-08-06'\n    url: https://id.hadron.ad.gt/api/v1/pbhid?partner_id=0&_it=prebid&t=1&src=id&domain=example.com\n    http_status: 200\n    note: >-\n      Returned application/json with a freshly minted hadronId for an anonymous\n      caller with partner_id=0 and no credential of any kind. Response values are\n      per-browser identifiers and are deliberately not recorded here.\n\n- id: console_session\n  type: session\n  in: cookie\n  secret: true\n  applies_to:\n  - https://api.audigent.com\n  - https://admin.audigent.com\n\
  \  description: >-\n    Customer/partner console login. The API host runs gunicorn behind a Django\n    stack and issues a 302 to https://admin.audigent.com for anonymous requests;\n    response headers advertise session cookie handling (Vary: Origin, Cookie),\n    X-Frame-Options DENY and Cross-Origin-Opener-Policy same-origin. No public\n    sign-up, no documented token endpoint, no OAuth metadata.\n  x-evidence:\n    fetched: '2026-08-06'\n    url: https://api.audigent.com/\n    http_status: 302\n    location: https://admin.audigent.com\n\nno_oauth: true\nno_oauth_reason: >-\n  No oauth2 or openIdConnect surface exists. /.well-known/oauth-authorization-server\n  and /.well-known/openid-configuration returned 404 on every Audigent and Hadron\n  host probed (id.hadron.ad.gt, analytics.hadron.ad.gt, seg.hadron.ad.gt,\n  cdn.hadronid.net, api.audigent.com). scopes/ is therefore correctly absent.\n\ncors:\n  access_control_allow_origin: '*'\n  access_control_allow_methods: GET, POST, OPTIONS\n\
  \  access_control_allow_headers: '*'\n  observed_on: https://id.hadron.ad.gt/api/v1/pbhid\n  note: >-\n    Fully open CORS on the identity endpoint, consistent with a surface intended\n    to be called from any publisher page.\n\nconsent_as_access_control:\n  note: >-\n    In place of authentication, the public endpoints gate behavior on privacy\n    consent signals passed by the page. See conformance/audigent-conformance.yml.\n  parameters:\n  - gdpr\n  - gdprString\n  - us_privacy\n  - gpp\n  - gpp_sid\n\ngaps:\n- No published authentication documentation on any Audigent-owned host.\n- No API-key or credential self-service; partner IDs are issued via sales/onboarding.\n- No machine-readable security scheme (no OpenAPI securitySchemes to derive from).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audigent/refs/heads/main/authentication/audigent-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Advertising
- AdTech
- Data
- Identity
- Programmatic
- Audience
- Marketing
- Privacy
- Prebid
- Header Bidding
- Data Curation
---
