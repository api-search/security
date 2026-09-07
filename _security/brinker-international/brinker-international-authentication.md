---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Brinker International Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brinker International declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Brinker International
provider_slug: brinker-international
scheme_count: 0
schemes: []
slug: brinker-international-authentication
source_filename: brinker-international-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://developer.brinker.com/portals/api/sites/brinker-portal/liveportal/page/faqs\ndocs: https://developer.brinker.com/faqs\nnote: >-\n  Brinker publishes no OpenAPI, so this profile is read from the provider's own\n  developer-portal FAQ page (fetched anonymously through the portal's public page API\n  at /portals/api/sites/brinker-portal/liveportal/page/faqs, HTTP 200). Brinker runs a\n  Google Apigee Edge gateway at api.brinker.com and a Google Apigee Integrated\n  Developer Portal at developer.brinker.com. Credentials are Apigee developer-app\n  consumer key + secret, issued only after a human at the \"Brinker API Team\" approves\n  both the account and the app. No OAuth authorization server, no OIDC discovery\n  document and no scope reference is published anonymously on any Brinker host.\nplatform: Google Apigee Edge\ngateway_host: api.brinker.com\nportal_host: developer.brinker.com\nsecurity_schemes:\n  - id: apigee-app-key\n\
  \    type: apiKey\n    name: API Key (Apigee developer-app consumer key)\n    location: unknown\n    description: >-\n      The FAQ states that after a developer app is created and Brinker activates the\n      credentials, \"you can see App details, API Keys and secrets\" — the standard Apigee\n      consumer key / consumer secret pair. The header or query parameter the key is\n      presented in is not documented anonymously; it is inside the gated API reference.\n    evidence: https://developer.brinker.com/faqs\n    verified: false\n    note: Scheme inferred from the provider's own FAQ prose plus the Apigee platform, not from a published contract.\nonboarding:\n  self_service: false\n  steps:\n    - Create an account at https://developer.brinker.com/accounts/create (a distribution list or shared mailbox is recommended for organizations).\n    - Receive a welcome email stating the account is created PENDING APPROVAL.\n    - Wait for the Brinker API Team to approve the account, then reset\
  \ the password via the emailed link.\n    - Sign in, create a developer app under Apps, and request Default Product access.\n    - 'API Product is assigned from the backend based on your entitlement (portal FAQ wording) — notify the Brinker API Team so they activate the credentials.'\n    - After approval, App details, API keys and secrets become visible.\n  approval_required: true\n  approver: Brinker API Team\n  entitlement_based: true\n  source: https://developer.brinker.com/faqs\noauth:\n  present: false\n  note: >-\n    No /.well-known/oauth-authorization-server, /.well-known/openid-configuration or\n    /.well-known/oauth-protected-resource is served on any Brinker host (see\n    well-known/brinker-international-well-known.yml). scopes/ is therefore not written —\n    there is no OAuth scope surface to derive or search.\nmtls:\n  present: false\nobserved_api_product_categories:\n  note: >-\n    The portal's anonymous catalog endpoint /portals/api/sites/<site>/liveportal/apis\n  \
  \  returns HTTP 200. On the production site (brinker-portal) it returns\n    apiDocs: [], apiProducts: [], apiCategoryList: [] — nothing at all is published to\n    anonymous visitors. On the QA site (brinkerqa-portal) the same endpoint returns\n    empty apiDocs/apiProducts but a populated apiCategoryList naming six API product\n    families. Those are CATEGORY NAMES published by Brinker's own portal, not contracts:\n    no path, operation, schema or base URL is exposed anonymously.\n  source: https://developerqa.brinker.com/portals/api/sites/brinkerqa-portal/liveportal/apis\n  http_status: 200\n  categories:\n    - LoyaltyEA\n    - Promos\n    - ITSM ServiceNow\n    - GMS\n    - OrderManagement\n    - POS\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brinker-international/refs/heads/main/authentication/brinker-international-authentication.yml
summary_line: 0 schemes
tags:
- Restaurant
- Casual Dining
- Food Service
- Franchise
- Chilis
- Maggianos
- Fortune 1000
---
