---
api_key_in: []
auth_types: []
description: Clicktivated publishes no authentication documentation, issues no public API credentials, and exposes no OAuth or OIDC metadata. The only authentication surface is the login on its customer dashboard, which sits behind a Cloudflare managed challenge. Nothing here is derived from a spec — there is no spec.
kind: authentication
layout: security
method: probed
name: Clicktivated Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clicktivated declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Clicktivated
provider_slug: clicktivated
scheme_count: 0
schemes: []
slug: clicktivated-authentication
source_filename: clicktivated-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live probes of api.clicktivatedstudio.com and dashboard.clicktivatedstudio.com\ndescription: >-\n  Clicktivated publishes no authentication documentation, issues no public API\n  credentials, and exposes no OAuth or OIDC metadata. The only authentication surface is\n  the login on its customer dashboard, which sits behind a Cloudflare managed challenge.\n  Nothing here is derived from a spec — there is no spec.\n\npointer_policy: >-\n  NO type: Authentication pointer is emitted in apis.yml. That pointer is a scored\n  assertion that the provider documents its authentication, and this artifact records\n  the opposite — scheme_count is 0 and no auth documentation exists on any Clicktivated\n  surface. The file is a measured absence, kept for auditability and cross-linked from\n  conventions/clicktivated-conventions.yml.\n\nschemes: []\nscheme_count: 0\ndocs: null\n\nfindings:\n- surface: graphql\n  url: https://api.clicktivatedstudio.com/graphql\n\
  \  auth_required: unknown\n  observed: >-\n    Anonymous requests reach the origin and are answered by Apollo's validation layer,\n    not by an authentication layer — a syntactically invalid field returned a schema\n    validation error rather than a 401 or 403. Whether individual fields are guarded\n    cannot be determined without knowing a valid operation, and the schema is not\n    readable.\n  status: 400\n- surface: graphql\n  control: Apollo CSRF prevention\n  detail: >-\n    Requests must carry a non-simple Content-Type (e.g. application/json) or one of\n    x-apollo-operation-name / apollo-require-preflight. This is a CSRF control, not\n    authentication.\n  status: 400\n- surface: dashboard\n  url: https://dashboard.clicktivatedstudio.com/login\n  auth_required: true\n  observed: >-\n    A customer login exists but is fronted by a Cloudflare managed challenge, so the\n    login mechanism itself was not observable.\n  status: 403\n- surface: player\n  url: https://player.clicktivatedstudio.com/watch?v=707975ec4b\n\
  \  auth_required: false\n  observed: >-\n    The embed player is fully anonymous. Access control is by possession of the opaque\n    10-hex-character video hash — a bearer-URL model with no expiry, no signature and no\n    revocation observable from outside.\n  status: 200\n\nfederation_metadata:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n  hosts_checked:\n  - clicktivated.com\n  - api.clicktivatedstudio.com\n  - player.clicktivatedstudio.com\n  - dashboard.clicktivatedstudio.com\n  note: See well-known/clicktivated-well-known.yml for the full probe matrix.\n\napi_keys:\n  issued_publicly: false\n  note: >-\n    No developer portal, no key-issuance flow, no key prefix convention, and no\n    documentation of any credential. Clicktivated's own how-it-works page tells customers\n    the product needs \"no complex API setups\".\n\nchecked: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clicktivated/refs/heads/main/authentication/clicktivated-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Video
- Interactive Video
- Shoppable Video
- Advertising Technology
- First-Party Data
- Retail
- Tourism
---
