---
api_key_in:
- header
- query
api_specs:
- filename: applovin-ad-units-api-openapi.yml
  format: yaml
  label: AppLovin Ad Units API
  slug: applovin-ad-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-ad-units-api-openapi.yml
- filename: applovin-asset-reporting-api-openapi.yml
  format: yaml
  label: AppLovin Asset Reporting API
  slug: applovin-asset-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-asset-reporting-api-openapi.yml
- filename: applovin-assets-api-openapi.yml
  format: yaml
  label: AppLovin Assets API
  slug: applovin-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-assets-api-openapi.yml
- filename: applovin-campaigns-api-openapi.yml
  format: yaml
  label: AppLovin Campaigns API
  slug: applovin-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-campaigns-api-openapi.yml
- filename: applovin-conversion-events-api-openapi.yml
  format: yaml
  label: AppLovin Conversion Events API
  slug: applovin-conversion-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-conversion-events-api-openapi.yml
- filename: applovin-creative-sets-api-openapi.yml
  format: yaml
  label: AppLovin Creative Sets API
  slug: applovin-creative-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-creative-sets-api-openapi.yml
- filename: applovin-experiments-api-openapi.yml
  format: yaml
  label: AppLovin Experiments API
  slug: applovin-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-experiments-api-openapi.yml
- filename: applovin-growth-reporting-api-openapi.yml
  format: yaml
  label: AppLovin Growth Reporting API
  slug: applovin-growth-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-growth-reporting-api-openapi.yml
- filename: applovin-revenue-reporting-api-openapi.yml
  format: yaml
  label: AppLovin Revenue Reporting API
  slug: applovin-revenue-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-revenue-reporting-api-openapi.yml
- filename: applovin-test-devices-api-openapi.yml
  format: yaml
  label: AppLovin Test Devices API
  slug: applovin-test-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-test-devices-api-openapi.yml
- filename: applovin-waterfalls-api-openapi.yml
  format: yaml
  label: AppLovin Waterfalls API
  slug: applovin-waterfalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/openapi/applovin-waterfalls-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Applovin Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppLovin secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AppLovin
provider_slug: applovin
scheme_count: 3
schemes:
- description: Campaign Management API key passed in the `Authorization` header.
  name: bearerAuth
  note: Modelled as http/bearer in the spec, but AppLovin's documented examples send the raw key with no `Bearer ` prefix. Treat as an opaque Authorization-header credential.
  scheme: bearer
  sources:
  - openapi/applovin-campaigns-api-openapi.yml
  - openapi/applovin-creative-sets-api-openapi.yml
  - openapi/applovin-assets-api-openapi.yml
  - openapi/applovin-conversion-events-api-openapi.yml
  type: http
- description: Report Key.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/applovin-revenue-reporting-api-openapi.yml
  - openapi/applovin-growth-reporting-api-openapi.yml
  - openapi/applovin-asset-reporting-api-openapi.yml
  type: apiKey
- description: Management Key from the AppLovin dashboard (Account > General > Keys).
  in: header
  name: apiKeyHeader
  parameter: Api-Key
  sources:
  - openapi/applovin-ad-units-api-openapi.yml
  - openapi/applovin-waterfalls-api-openapi.yml
  - openapi/applovin-experiments-api-openapi.yml
  - openapi/applovin-test-devices-api-openapi.yml
  type: apiKey
slug: applovin-authentication
source_filename: applovin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/*.yml + provider documentation\ndocs:\n- https://support.applovin.com/en/app-discovery/api/axon-campaign-management-api/\n- https://support.applovin.com/en/max/advanced-features/ad-unit-management-api\n- https://support.applovin.com/en/max/reporting-apis/revenue-reporting-api\n- https://support.applovin.com/en/growth/promoting-your-websites/api/conversion-api-for-lead-gen\n- https://support.applovin.com/en/max/ad-review/rules-management-api\nnote: >-\n  Upgraded from derived to searched on 2026-08-13. The derived pass read three security\n  schemes out of the OpenAPI. The documentation shows the real model is worse than the\n  spec suggests: AppLovin issues SIX distinct, non-interchangeable, account-wide static\n  keys across five products, in three different transport locations, with no OAuth, no\n  scopes, no expiry and no programmatic rotation. A 401 on a well-formed AppLovin request\n  is usually the right key sent\
  \ to the wrong product.\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header, query]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  distinct_credentials: 6\n  key_issuance: 'AppLovin dashboard, Account > General > Keys'\n  dashboard: https://max.applovin.com/login\ncredentials:\n- name: Campaign Management API key\n  product: Axon Campaign Management API\n  transport: header\n  parameter: Authorization\n  format: raw key, no Bearer prefix\n  additional_required: 'account_id query parameter on every request'\n  hosts: [api.ads.axon.ai]\n  scheme: bearerAuth\n  docs: https://support.applovin.com/en/app-discovery/api/axon-campaign-management-api/\n  note: >-\n    The docs explicitly warn this is a different key from the Management key used by the\n    Ad Unit Management API.\n- name: Management Key\n  product: MAX Ad Unit Management API\n  transport: header\n  parameter: Api-Key\n  hosts: [o.applovin.com]\n  scheme: apiKeyHeader\n  docs: https://support.applovin.com/en/max/advanced-features/ad-unit-management-api\n\
  - name: Report Key\n  product: Reporting family (revenue, growth, asset, cohort, web, user-level)\n  transport: query\n  parameter: api_key\n  hosts: [r.applovin.com]\n  scheme: apiKeyQuery\n  docs: https://support.applovin.com/en/max/reporting-apis/revenue-reporting-api\n  risk: >-\n    A long-lived account-wide credential carried in the QUERY STRING of every reporting\n    request. It will appear in web-server access logs, proxy logs, CDN logs and any\n    shell history that contains the curl command. AppLovin publishes no header-based\n    alternative for the reporting hosts.\n- name: Conversion API key\n  product: Conversion API (web events)\n  transport: header\n  parameter: Authorization\n  additional_required: 'pixel_id query parameter carrying the AppLovin Event Key'\n  hosts: [b.applovin.com]\n  docs: https://support.applovin.com/en/growth/promoting-your-websites/api/conversion-api-for-lead-gen\n- name: Ad Review Key\n  product: Ad Review Rules Management API\n  transport: header\n\
  \  parameter: Api-Key\n  hosts: [api-safedk.applovin.com]\n  docs: https://support.applovin.com/en/max/ad-review/rules-management-api\n  note: Same header NAME as the MAX Management Key, different credential value and different host.\n- name: SDK Key / Event Key\n  product: MAX client SDKs and server-to-server callbacks\n  transport: embedded in the mobile app / used as a hashing secret\n  docs: https://support.applovin.com/en/max/faq/how-server-to-server-callback-works\n  note: >-\n    The Event Key is not an API credential — it is the shared secret AppLovin hashes with\n    an event ID to produce the {EVENT_TOKEN} macro on rewarded callbacks,\n    sha1(EVENT_ID + EVENT_KEY). Recorded here because it is issued from the same Keys page\n    and is routinely confused with the API keys.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Campaign Management API key passed in the `Authorization` header.\n  sources:\n  - openapi/applovin-campaigns-api-openapi.yml\n\
  \  - openapi/applovin-creative-sets-api-openapi.yml\n  - openapi/applovin-assets-api-openapi.yml\n  - openapi/applovin-conversion-events-api-openapi.yml\n  note: >-\n    Modelled as http/bearer in the spec, but AppLovin's documented examples send the raw\n    key with no `Bearer ` prefix. Treat as an opaque Authorization-header credential.\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Report Key.\n  sources:\n  - openapi/applovin-revenue-reporting-api-openapi.yml\n  - openapi/applovin-growth-reporting-api-openapi.yml\n  - openapi/applovin-asset-reporting-api-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: Management Key from the AppLovin dashboard (Account > General > Keys).\n  sources:\n  - openapi/applovin-ad-units-api-openapi.yml\n  - openapi/applovin-waterfalls-api-openapi.yml\n  - openapi/applovin-experiments-api-openapi.yml\n  - openapi/applovin-test-devices-api-openapi.yml\nagent_readiness:\n\
  \  scoped_credentials: false\n  short_lived_tokens: false\n  programmatic_rotation: false\n  revocation_api: false\n  least_privilege: false\n  assessment: >-\n    Every AppLovin credential is a long-lived, account-wide, full-privilege static key with\n    no expiry and no API-driven rotation or revocation. There is no read-only variant of\n    any key: the Management Key that lists ad units is the same key that rewrites their\n    waterfalls, and the Campaign Management key that lists campaigns is the same key that\n    creates them and spends money. An agent cannot be given a narrower credential than a\n    human employee, which makes delegation to an autonomous agent an all-or-nothing\n    decision.\ngaps:\n- No OAuth 2.0, no OpenID Connect, no token endpoint, no /.well-known/oauth-authorization-server (probed, 404/400 on every API host).\n- No scopes, so scopes/applovin-scopes.yml is intentionally not emitted.\n- No mTLS.\n- No key expiry or rotation API; rotation is a manual dashboard\
  \ action.\n- Report Key travels in the query string.\n- Same header name (Api-Key) reused for two different credentials on two different hosts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/applovin/refs/heads/main/authentication/applovin-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Advertising
- Mobile
- AdTech
- App Monetization
- Mediation
- User Acquisition
- Marketing Technology
- Conversion Tracking
---
