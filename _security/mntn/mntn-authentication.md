---
api_key_in:
- header
- query
api_specs:
- filename: mntn-reporting-api-openapi.yml
  format: yaml
  label: MNTN Reporting API 3.0
  slug: mntn-reporting-api-30
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-reporting-api-openapi.yml
- filename: mntn-advertisers-api-openapi.yml
  format: yaml
  label: MNTN Advertisers API
  slug: mntn-advertisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-advertisers-api-openapi.yml
- filename: mntn-api-api-openapi.yml
  format: yaml
  label: MNTN API
  slug: mntn-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-api-api-openapi.yml
- filename: mntn-attribution-api-openapi.yml
  format: yaml
  label: MNTN Attribution API
  slug: mntn-attribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-attribution-api-openapi.yml
- filename: mntn-audiences-api-openapi.yml
  format: yaml
  label: MNTN Audiences API
  slug: mntn-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-audiences-api-openapi.yml
- filename: mntn-batch-api-openapi.yml
  format: yaml
  label: MNTN Batch API
  slug: mntn-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-batch-api-openapi.yml
- filename: mntn-campaigns-api-openapi.yml
  format: yaml
  label: MNTN Campaigns API
  slug: mntn-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-campaigns-api-openapi.yml
- filename: mntn-creatives-api-openapi.yml
  format: yaml
  label: MNTN Creatives API
  slug: mntn-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-creatives-api-openapi.yml
- filename: mntn-flights-api-openapi.yml
  format: yaml
  label: MNTN Flights API
  slug: mntn-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-flights-api-openapi.yml
- filename: mntn-organizations-api-openapi.yml
  format: yaml
  label: MNTN Organizations API
  slug: mntn-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-organizations-api-openapi.yml
- filename: mntn-pixel-api-openapi.yml
  format: yaml
  label: MNTN Pixel API
  slug: mntn-pixel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-pixel-api-openapi.yml
- filename: mntn-pmp-campaign-deals-api-openapi.yml
  format: yaml
  label: MNTN Pmp Campaign Deals API
  slug: mntn-pmp-campaign-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-pmp-campaign-deals-api-openapi.yml
- filename: mntn-pmp-channels-api-openapi.yml
  format: yaml
  label: MNTN Pmp Channels API
  slug: mntn-pmp-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-pmp-channels-api-openapi.yml
- filename: mntn-pmp-deal-groups-api-openapi.yml
  format: yaml
  label: MNTN Pmp Deal Groups API
  slug: mntn-pmp-deal-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-pmp-deal-groups-api-openapi.yml
- filename: mntn-pmp-deals-api-openapi.yml
  format: yaml
  label: MNTN Pmp Deals API
  slug: mntn-pmp-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-pmp-deals-api-openapi.yml
- filename: mntn-pmp-partners-api-openapi.yml
  format: yaml
  label: MNTN Pmp Partners API
  slug: mntn-pmp-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-pmp-partners-api-openapi.yml
- filename: mntn-reference-api-openapi.yml
  format: yaml
  label: MNTN Reference API
  slug: mntn-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/openapi/mntn-reference-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Mntn Authentication
name_suffix: Authentication
oauth_flows: []
overview: MNTN secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MNTN
provider_slug: mntn
scheme_count: 3
schemes:
- description: MNTN-issued advertiser API key. Available in Account Settings.
  in: query
  name: API Key
  parameter: key
  sources:
  - openapi/mntn-batch-export-openapi.yml
  - openapi/mntn-reporting-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: Bearer
  scheme: bearer
  sources:
  - openapi/mntn-ptv-advertisers-openapi.yml
  - openapi/mntn-ptv-attribution-openapi.yml
  - openapi/mntn-ptv-audiences-openapi.yml
  - openapi/mntn-ptv-campaigns-openapi.yml
  - openapi/mntn-ptv-creatives-openapi.yml
  - openapi/mntn-ptv-flights-openapi.yml
  - openapi/mntn-ptv-organizations-openapi.yml
  - openapi/mntn-ptv-pixel-openapi.yml
  - openapi/mntn-ptv-pmp-campaign-deals-openapi.yml
  - openapi/mntn-ptv-pmp-channels-openapi.yml
  - openapi/mntn-ptv-pmp-deal-groups-openapi.yml
  - openapi/mntn-ptv-pmp-deals-openapi.yml
  - openapi/mntn-ptv-pmp-partners-openapi.yml
  - openapi/mntn-ptv-reference-openapi.yml
  - openapi/mntn-ptv-reporting-openapi.yml
  type: http
- in: header
  name: API Key
  parameter: X-API-Key
  sources:
  - openapi/mntn-ptv-advertisers-openapi.yml
  - openapi/mntn-ptv-attribution-openapi.yml
  - openapi/mntn-ptv-audiences-openapi.yml
  - openapi/mntn-ptv-campaigns-openapi.yml
  - openapi/mntn-ptv-creatives-openapi.yml
  - openapi/mntn-ptv-flights-openapi.yml
  - openapi/mntn-ptv-organizations-openapi.yml
  - openapi/mntn-ptv-pixel-openapi.yml
  - openapi/mntn-ptv-pmp-campaign-deals-openapi.yml
  - openapi/mntn-ptv-pmp-channels-openapi.yml
  - openapi/mntn-ptv-pmp-deal-groups-openapi.yml
  - openapi/mntn-ptv-pmp-deals-openapi.yml
  - openapi/mntn-ptv-pmp-partners-openapi.yml
  - openapi/mntn-ptv-reference-openapi.yml
  - openapi/mntn-ptv-reporting-openapi.yml
  type: apiKey
slug: mntn-authentication
source_filename: mntn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\ndocs:\n- https://help.mountain.com/en/articles/6511970-access-your-reporting-api-key\n- https://api.mountain.com/docs\n- https://api3.mountain.com/docs\nsource: openapi/mntn-batch-export-openapi.yml, openapi/mntn-ptv-advertisers-openapi.yml, openapi/mntn-ptv-attribution-openapi.yml,\n  openapi/mntn-ptv-audiences-openapi.yml, openapi/mntn-ptv-campaigns-openapi.yml, openapi/mntn-ptv-creatives-openapi.yml,\n  openapi/mntn-ptv-flights-openapi.yml, openapi/mntn-ptv-organizations-openapi.yml, openapi/mntn-ptv-pixel-openapi.yml,\n  openapi/mntn-ptv-pmp-campaign-deals-openapi.yml, openapi/mntn-ptv-pmp-channels-openapi.yml,\n  openapi/mntn-ptv-pmp-deal-groups-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: API Key\n  type: apiKey\n  in: query\n  parameter: key\n  description: MNTN-issued advertiser API key. Available in Account Settings.\n  sources:\n  - openapi/mntn-batch-export-openapi.yml\n\
  \  - openapi/mntn-reporting-api-openapi.yml\n- name: Bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/mntn-ptv-advertisers-openapi.yml\n  - openapi/mntn-ptv-attribution-openapi.yml\n  - openapi/mntn-ptv-audiences-openapi.yml\n  - openapi/mntn-ptv-campaigns-openapi.yml\n  - openapi/mntn-ptv-creatives-openapi.yml\n  - openapi/mntn-ptv-flights-openapi.yml\n  - openapi/mntn-ptv-organizations-openapi.yml\n  - openapi/mntn-ptv-pixel-openapi.yml\n  - openapi/mntn-ptv-pmp-campaign-deals-openapi.yml\n  - openapi/mntn-ptv-pmp-channels-openapi.yml\n  - openapi/mntn-ptv-pmp-deal-groups-openapi.yml\n  - openapi/mntn-ptv-pmp-deals-openapi.yml\n  - openapi/mntn-ptv-pmp-partners-openapi.yml\n  - openapi/mntn-ptv-reference-openapi.yml\n  - openapi/mntn-ptv-reporting-openapi.yml\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/mntn-ptv-advertisers-openapi.yml\n  - openapi/mntn-ptv-attribution-openapi.yml\n  - openapi/mntn-ptv-audiences-openapi.yml\n\
  \  - openapi/mntn-ptv-campaigns-openapi.yml\n  - openapi/mntn-ptv-creatives-openapi.yml\n  - openapi/mntn-ptv-flights-openapi.yml\n  - openapi/mntn-ptv-organizations-openapi.yml\n  - openapi/mntn-ptv-pixel-openapi.yml\n  - openapi/mntn-ptv-pmp-campaign-deals-openapi.yml\n  - openapi/mntn-ptv-pmp-channels-openapi.yml\n  - openapi/mntn-ptv-pmp-deal-groups-openapi.yml\n  - openapi/mntn-ptv-pmp-deals-openapi.yml\n  - openapi/mntn-ptv-pmp-partners-openapi.yml\n  - openapi/mntn-ptv-reference-openapi.yml\n  - openapi/mntn-ptv-reporting-openapi.yml\n\nkey_issuance:\n  self_service: true\n  where: MNTN platform UI, My Account / Account Settings -> API tab\n  docs: https://help.mountain.com/en/articles/6511970-access-your-reporting-api-key\n  note: >-\n    MNTN issues one advertiser-scoped Reporting API key per account from the platform UI. The help\n    center instructs customers to \"treat it like a password and only share it with platforms you\n    trust\" -- there is no published key rotation,\
  \ expiry, or scoping model, and no OAuth 2.0 or\n    OpenID Connect surface is documented on any MNTN host.\nsurfaces:\n- api: MNTN Performance TV (PTV) API\n  host: https://api.mountain.com\n  accepted:\n  - {scheme: Bearer, transport: 'Authorization: Bearer <JWT>', format: JWT}\n  - {scheme: API Key, transport: 'X-API-Key: <key>', format: opaque}\n  unauthenticated_behavior:\n    status: 401\n    body: '{\"error\":\"Authentication required\"}'\n    content_type: application/json\n    note: >-\n      The api.mountain.com gateway (istio-envoy) answers 401 for every path except /openapi.json,\n      /openapi.yaml and /docs, which are served anonymously.\n- api: MNTN Reporting API 3.0 and Async Batch Export API\n  host: https://api3.mountain.com\n  accepted:\n  - {scheme: API Key, transport: 'key=<key> query parameter', format: opaque}\n  unauthenticated_behavior:\n    status: 401\n    body: RFC 9457 application/problem+json\n  note: >-\n    The reporting API carries the credential in the\
  \ URL query string, which leaks the key into proxy\n    logs, browser history, and referrer headers. A header-borne alternative is not documented.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes: none published\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mntn/refs/heads/main/authentication/mntn-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- connected-tv
- ctv-advertising
- Advertising
- performance-marketing
- streaming-tv
- media-buying
- Attribution
- audience-targeting
- conversion-tracking
- programmatic-advertising
- private-marketplace
- marketing-reporting
- adtech
---
