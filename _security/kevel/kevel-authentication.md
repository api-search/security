---
api_key_in:
- header
api_specs:
- filename: kevel-ads-api-openapi.yml
  format: yaml
  label: Kevel Ads API
  slug: kevel-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-ads-api-openapi.yml
- filename: kevel-advertisers-api-openapi.yml
  format: yaml
  label: Kevel Advertisers API
  slug: kevel-advertisers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-advertisers-api-openapi.yml
- filename: kevel-campaigns-api-openapi.yml
  format: yaml
  label: Kevel Campaigns API
  slug: kevel-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-campaigns-api-openapi.yml
- filename: kevel-channels-api-openapi.yml
  format: yaml
  label: Kevel Channels API
  slug: kevel-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-channels-api-openapi.yml
- filename: kevel-creatives-api-openapi.yml
  format: yaml
  label: Kevel Creatives API
  slug: kevel-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-creatives-api-openapi.yml
- filename: kevel-decision-api-openapi.yml
  format: yaml
  label: Kevel Decision API
  slug: kevel-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-decision-api-openapi.yml
- filename: kevel-flights-api-openapi.yml
  format: yaml
  label: Kevel Flights API
  slug: kevel-flights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-flights-api-openapi.yml
- filename: kevel-reporting-api-openapi.yml
  format: yaml
  label: Kevel Reporting API
  slug: kevel-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-reporting-api-openapi.yml
- filename: kevel-sites-api-openapi.yml
  format: yaml
  label: Kevel Sites API
  slug: kevel-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-sites-api-openapi.yml
- filename: kevel-zones-api-openapi.yml
  format: yaml
  label: Kevel Zones API
  slug: kevel-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/openapi/kevel-zones-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kevel/refs/heads/main/authentication/kevel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Ad Serving
- Advertising
- API-First
- Audience
- Monetization
- Reporting
---
