---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Department Of Housing And Urban Development Authentication
name_suffix: Authentication
oauth_flows: []
overview: Department of Housing and Urban Development declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Department of Housing and Urban Development
provider_slug: department-of-housing-and-urban-development
scheme_count: 0
schemes: []
slug: department-of-housing-and-urban-development-authentication
source_filename: department-of-housing-and-urban-development-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://www.huduser.gov/portal/dataset/fmr-api.html,\n  https://www.huduser.gov/portal/dataset/uspszip-api.html,\n  https://www.huduser.gov/portal/dataset/chas-api.html,\n  https://www.huduser.gov/portal/dataset/api-terms-of-service.html\n  (all fetched 2026-09-06, HTTP 200), plus a live anonymous probe of\n  https://www.huduser.gov/hudapi/public/fmr/listStates (HTTP 401\n  {\"error\":\"Unauthenticated\"}).\nprovider: Department of Housing and Urban Development\nproviderId: department-of-housing-and-urban-development\ndocs: https://www.huduser.gov/portal/dataset/fmr-api.html\nsummary: >-\n  HUD's public API surface uses three different and unrelated access models.\n  The HUD USER Datasets API (FMR, IL, MTSP-IL, CHAS, USPS Crosswalk) requires a\n  bearer access token issued from a free HUD USER account, and authorization is\n  granted PER DATASET — a valid token still returns 403 for a dataset the\n  account did not register\
  \ for. The eGIS ArcGIS REST services and the\n  data.hud.gov open-data catalog are anonymous and unauthenticated. There is no\n  OAuth 2.0, no OpenID Connect, no mTLS and no scope surface anywhere on the\n  HUD API estate.\napis:\n  - api: HUD USER FMR/IL API\n    baseURL: https://www.huduser.gov/hudapi/public\n    schemes:\n      - id: hudUserBearerToken\n        type: http\n        scheme: bearer\n        in: header\n        header: Authorization\n        format: 'Authorization: Bearer <access token>'\n        token_type: opaque access token (not a JWT the docs describe or verify)\n        issuance: >-\n          Register a free account at https://www.huduser.gov/hudapi/public/register,\n          confirm it by email, log in, select the Datasets APIs you want access\n          to, then click \"Create New Token\".\n        registration_url: https://www.huduser.gov/hudapi/public/register\n        login_url: https://www.huduser.gov/hudapi/public/login\n        cost: free\n        rotation:\
  \ >-\n          Tokens are created and revoked by the account holder from the HUD USER\n          Datasets API account page. No expiry or rotation period is documented.\n        per_dataset_authorization: true\n        per_dataset_note: >-\n          The published response-code table states 403 means \"Not allowed to\n          access this dataset API because you have not registered for it\" — a\n          per-dataset entitlement check that is distinct from 401\n          authentication failure. An agent holding a working token can still be\n          refused a dataset.\n        verified:\n          url: https://www.huduser.gov/hudapi/public/fmr/listStates\n          method: GET\n          anonymous: true\n          status: 401\n          body: '{\"error\":\"Unauthenticated\"}'\n          fetched: '2026-09-06'\n  - api: HUD eGIS ArcGIS REST Services\n    baseURL: https://egis.hud.gov/ArcGIS/rest/services\n    schemes:\n      - id: none\n        type: none\n        description: >-\n   \
  \       Anonymous public read. The ArcGIS Server service directory, service\n          metadata and query endpoints answered 200 with no credential on\n          2026-09-06.\n        verified:\n          url: https://egis.hud.gov/ArcGIS/rest/services?f=json\n          method: GET\n          anonymous: true\n          status: 200\n          fetched: '2026-09-06'\n  - api: HUD Open Data Catalog\n    baseURL: https://data.hud.gov\n    schemes:\n      - id: none\n        type: none\n        description: >-\n          Anonymous public read of the DCAT-US 1.1 catalog document.\n        verified:\n          url: https://data.hud.gov/data.json\n          method: GET\n          anonymous: true\n          status: 200\n          fetched: '2026-09-06'\n  - api: FHA Mortgage Limits\n    baseURL: https://entp.hud.gov\n    schemes:\n      - id: none\n        type: none\n        description: >-\n          Anonymous public HTML lookup form. No documented programmatic\n          credential, and no machine-readable\
  \ contract.\n        verified:\n          url: https://entp.hud.gov/idapp/html/hicostlook.cfm\n          method: GET\n          anonymous: true\n          status: 200\n          fetched: '2026-09-06'\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes_surface: false\nscopes_note: >-\n  No OAuth 2.0 anywhere on the estate, so scopes/ is deliberately not written —\n  the per-dataset entitlement recorded above is the closest thing to a scope and\n  it is granted through the account UI, not through a token grant.\ngaps:\n  - No documented token lifetime, expiry or refresh procedure.\n  - >-\n    No published list of the dataset entitlement values an account can hold, so\n    a 403 cannot be resolved programmatically — only through the account UI.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-housing-and-urban-development/refs/heads/main/authentication/department-of-housing-and-urban-development-authentication.yml
summary_line: 0 schemes
tags:
- Affordable Housing
- Fair Market Rents
- Federal-Government
- FHA
- GIS
- Housing
- HUD
- Income Limits
- Mortgage
- Open Data
---
