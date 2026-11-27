---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kaminari-ad-account-api-openapi.yml
  format: yaml
  label: Kaminari Ad Account API
  slug: kaminari-ad-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-account-api-openapi.yml
- filename: kaminari-ad-alert-notifications-api-openapi.yml
  format: yaml
  label: Kaminari Ad Alert Notifications API
  slug: kaminari-ad-alert-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-alert-notifications-api-openapi.yml
- filename: kaminari-ad-alerts-api-openapi.yml
  format: yaml
  label: Kaminari Ad Alerts API
  slug: kaminari-ad-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-alerts-api-openapi.yml
- filename: kaminari-ad-billing-api-openapi.yml
  format: yaml
  label: Kaminari Ad Billing API
  slug: kaminari-ad-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-billing-api-openapi.yml
- filename: kaminari-ad-campaign-groups-api-openapi.yml
  format: yaml
  label: Kaminari Ad Campaign Groups API
  slug: kaminari-ad-campaign-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-campaign-groups-api-openapi.yml
- filename: kaminari-ad-campaigns-api-openapi.yml
  format: yaml
  label: Kaminari Ad Campaigns API
  slug: kaminari-ad-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-campaigns-api-openapi.yml
- filename: kaminari-ad-custom-rules-api-openapi.yml
  format: yaml
  label: Kaminari Ad Custom Rules API
  slug: kaminari-ad-custom-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-custom-rules-api-openapi.yml
- filename: kaminari-ad-custom-taxonomies-api-openapi.yml
  format: yaml
  label: Kaminari Ad Custom Taxonomies API
  slug: kaminari-ad-custom-taxonomies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-custom-taxonomies-api-openapi.yml
- filename: kaminari-ad-emulators-api-openapi.yml
  format: yaml
  label: Kaminari Ad Emulators API
  slug: kaminari-ad-emulators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-emulators-api-openapi.yml
- filename: kaminari-ad-geos-api-openapi.yml
  format: yaml
  label: Kaminari Ad Geos API
  slug: kaminari-ad-geos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-geos-api-openapi.yml
- filename: kaminari-ad-invoicing-api-openapi.yml
  format: yaml
  label: Kaminari Ad Invoicing API
  slug: kaminari-ad-invoicing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-invoicing-api-openapi.yml
- filename: kaminari-ad-policy-sets-api-openapi.yml
  format: yaml
  label: Kaminari Ad Policy Sets API
  slug: kaminari-ad-policy-sets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-policy-sets-api-openapi.yml
- filename: kaminari-ad-proxy-api-openapi.yml
  format: yaml
  label: Kaminari Ad Proxy API
  slug: kaminari-ad-proxy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-proxy-api-openapi.yml
- filename: kaminari-ad-runs-api-openapi.yml
  format: yaml
  label: Kaminari Ad Runs API
  slug: kaminari-ad-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-runs-api-openapi.yml
- filename: kaminari-ad-scans-api-openapi.yml
  format: yaml
  label: Kaminari Ad Scans API
  slug: kaminari-ad-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-scans-api-openapi.yml
- filename: kaminari-ad-tags-api-openapi.yml
  format: yaml
  label: Kaminari Ad Tags API
  slug: kaminari-ad-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-tags-api-openapi.yml
- filename: kaminari-ad-webhooks-api-openapi.yml
  format: yaml
  label: Kaminari Ad Webhooks API
  slug: kaminari-ad-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kaminari-ad/openapi/kaminari-ad-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for Kaminari Ad API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kaminari Ad Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kaminari Ad declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kaminari Ad
provider_slug: kaminari-ad
scheme_count: 1
schemes:
- evidence: 'For server-to-server automation, create an API key under Account -> API Keys and send it as a Bearer token: curl https://app.kaminari.ad/api/v1/scans/<scan_id> \ -H "Authorization: Bearer $KAM_API_KEY"'
  header: Authorization
  how_to_obtain: Create an API key in the dashboard under Account → API Keys.
  location: header
  name: API Key
  type: http-bearer
slug: kaminari-ad-authentication
source_filename: kaminari-ad-authentication.yml
source_heading: Authentication Profile
source_url: https://kaminari.ad/docs/platform/authentication
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kaminari.ad/docs/platform/authentication\nsources:\n- https://kaminari.ad/docs/platform/authentication\n- https://kaminari.ad/docs/ui-reference/authentication-screens\n- https://kaminari.ad/docs/developers/authentication\n- https://kaminari.ad/docs/developers/oauth-connected-apps\ndescription: Authentication schemes for Kaminari Ad API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'For server-to-server automation, create an API key under Account -> API Keys and send it as a Bearer token: curl https://app.kaminari.ad/api/v1/scans/<scan_id>\n    \\ -H \"Authorization: Bearer $KAM_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the dashboard under Account → API Keys.\ndocs: https://kaminari.ad/docs/platform/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/kaminari-ad/authentication/kaminari-ad-authentication.yml
summary_line: 1 scheme
tags:
- Advertising
- Security
- Artificial Intelligence
- Fraud Prevention
- Real Devices
---
