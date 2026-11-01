---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: kevel-ad-api-openapi.yml
  format: yaml
  label: Kevel Ad API
  slug: kevel-ad-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-ad-api-openapi.yml
- filename: kevel-adtypes-api-openapi.yml
  format: yaml
  label: Kevel Adtypes API
  slug: kevel-adtypes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-adtypes-api-openapi.yml
- filename: kevel-advertiser-api-openapi.yml
  format: yaml
  label: Kevel Advertiser API
  slug: kevel-advertiser-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-advertiser-api-openapi.yml
- filename: kevel-campaign-api-openapi.yml
  format: yaml
  label: Kevel Campaign API
  slug: kevel-campaign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-campaign-api-openapi.yml
- filename: kevel-categories-api-openapi.yml
  format: yaml
  label: Kevel Categories API
  slug: kevel-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-categories-api-openapi.yml
- filename: kevel-category-catalog-api-openapi.yml
  format: yaml
  label: Kevel Category Catalog API
  slug: kevel-category-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-category-catalog-api-openapi.yml
- filename: kevel-channel-api-openapi.yml
  format: yaml
  label: Kevel Channel API
  slug: kevel-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-channel-api-openapi.yml
- filename: kevel-channelsinsite-api-openapi.yml
  format: yaml
  label: Kevel Channels In Site API
  slug: kevel-channelsinsite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-channelsinsite-api-openapi.yml
- filename: kevel-channelsite-api-openapi.yml
  format: yaml
  label: Kevel Channel Site API
  slug: kevel-channelsite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-channelsite-api-openapi.yml
- filename: kevel-countries-api-openapi.yml
  format: yaml
  label: Kevel Countries API
  slug: kevel-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-countries-api-openapi.yml
- filename: kevel-country-api-openapi.yml
  format: yaml
  label: Kevel Country API
  slug: kevel-country-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-country-api-openapi.yml
- filename: kevel-creative-api-openapi.yml
  format: yaml
  label: Kevel Creative API
  slug: kevel-creative-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-creative-api-openapi.yml
- filename: kevel-creative-templates-api-openapi.yml
  format: yaml
  label: Kevel Creative Templates API
  slug: kevel-creative-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-creative-templates-api-openapi.yml
- filename: kevel-entitycounts-api-openapi.yml
  format: yaml
  label: Kevel Entitycounts API
  slug: kevel-entitycounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-entitycounts-api-openapi.yml
- filename: kevel-fast-api-openapi.yml
  format: yaml
  label: Kevel Fast API
  slug: kevel-fast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-fast-api-openapi.yml
- filename: kevel-flight-api-openapi.yml
  format: yaml
  label: Kevel Flight API
  slug: kevel-flight-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-flight-api-openapi.yml
- filename: kevel-instantcounts-api-openapi.yml
  format: yaml
  label: Kevel Instantcounts API
  slug: kevel-instantcounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-instantcounts-api-openapi.yml
- filename: kevel-itemdb-api-openapi.yml
  format: yaml
  label: Kevel Itemdb API
  slug: kevel-itemdb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-itemdb-api-openapi.yml
- filename: kevel-login-api-openapi.yml
  format: yaml
  label: Kevel Login API
  slug: kevel-login-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-login-api-openapi.yml
- filename: kevel-priority-api-openapi.yml
  format: yaml
  label: Kevel Priority API
  slug: kevel-priority-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-priority-api-openapi.yml
- filename: kevel-region-api-openapi.yml
  format: yaml
  label: Kevel Region API
  slug: kevel-region-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-region-api-openapi.yml
- filename: kevel-segment-api-openapi.yml
  format: yaml
  label: Kevel Segment API
  slug: kevel-segment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-segment-api-openapi.yml
- filename: kevel-site-api-openapi.yml
  format: yaml
  label: Kevel Site API
  slug: kevel-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-site-api-openapi.yml
- filename: kevel-zone-api-openapi.yml
  format: yaml
  label: Kevel Zone API
  slug: kevel-zone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kevel/openapi/kevel-zone-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Kevel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kevel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kevel
provider_slug: kevel
scheme_count: 1
schemes:
- description: Management/Reporting API key issued from the Kevel UI.
  in: header
  name: ApiKeyAuth
  parameter: X-Adzerk-ApiKey
  sources:
  - openapi/kevel-openapi.yml
  type: apiKey
slug: kevel-authentication
source_filename: kevel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kevel-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Adzerk-ApiKey\n  description: Management/Reporting API key issued from the Kevel UI.\n  sources:\n  - openapi/kevel-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/kevel/authentication/kevel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Ad Serving
- Advertising
- API-First
- Audiences
- Monetization
- Reporting
---
