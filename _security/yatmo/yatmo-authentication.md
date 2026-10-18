---
anonymous_access: false
api_key_in: []
api_specs:
- filename: yatmo-bikepaths-api-openapi.yml
  format: yaml
  label: Yatmo Bike Paths API
  slug: yatmo-bikepaths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-bikepaths-api-openapi.yml
- filename: yatmo-categories-api-openapi.yml
  format: yaml
  label: Yatmo Categories API
  slug: yatmo-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-categories-api-openapi.yml
- filename: yatmo-enrichment-api-openapi.yml
  format: yaml
  label: Yatmo Enrichment API
  slug: yatmo-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-enrichment-api-openapi.yml
- filename: yatmo-frenchneighbourhoods-api-openapi.yml
  format: yaml
  label: Yatmo French Neighbourhoods API
  slug: yatmo-frenchneighbourhoods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-frenchneighbourhoods-api-openapi.yml
- filename: yatmo-geolocation-api-openapi.yml
  format: yaml
  label: Yatmo Geolocation API
  slug: yatmo-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-geolocation-api-openapi.yml
- filename: yatmo-geopositionencoder-api-openapi.yml
  format: yaml
  label: Yatmo Geo Position Encoder API
  slug: yatmo-geopositionencoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-geopositionencoder-api-openapi.yml
- filename: yatmo-image-api-openapi.yml
  format: yaml
  label: Yatmo Image API
  slug: yatmo-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-image-api-openapi.yml
- filename: yatmo-immotopcategories-api-openapi.yml
  format: yaml
  label: Yatmo Immotop Categories API
  slug: yatmo-immotopcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-immotopcategories-api-openapi.yml
- filename: yatmo-isochrone-api-openapi.yml
  format: yaml
  label: Yatmo Isochrone API
  slug: yatmo-isochrone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-isochrone-api-openapi.yml
- filename: yatmo-nearcheck-api-openapi.yml
  format: yaml
  label: Yatmo Near Check API
  slug: yatmo-nearcheck-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-nearcheck-api-openapi.yml
- filename: yatmo-neighbourhood-api-openapi.yml
  format: yaml
  label: Yatmo Neighbourhood API
  slug: yatmo-neighbourhood-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-neighbourhood-api-openapi.yml
- filename: yatmo-points-api-openapi.yml
  format: yaml
  label: Yatmo Points API
  slug: yatmo-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-points-api-openapi.yml
- filename: yatmo-route-api-openapi.yml
  format: yaml
  label: Yatmo Route API
  slug: yatmo-route-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-route-api-openapi.yml
- filename: yatmo-scores-api-openapi.yml
  format: yaml
  label: Yatmo Scores API
  slug: yatmo-scores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-scores-api-openapi.yml
- filename: yatmo-shape-api-openapi.yml
  format: yaml
  label: Yatmo Shape API
  slug: yatmo-shape-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-shape-api-openapi.yml
- filename: yatmo-simplifiedcategories-api-openapi.yml
  format: yaml
  label: Yatmo Simplified Categories API
  slug: yatmo-simplifiedcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-simplifiedcategories-api-openapi.yml
- filename: yatmo-summary-api-openapi.yml
  format: yaml
  label: Yatmo Summary API
  slug: yatmo-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/openapi/yatmo-summary-api-openapi.yml
auth_types: []
description: Yatmo uses API‑key authentication via HTTP headers. No OAuth flows are defined.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Yatmo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yatmo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Yatmo
provider_slug: yatmo
scheme_count: 2
schemes:
- evidence: Every request to the Yatmo API carries your backend license key in an HTTP header.
  header: LicenseKey
  how_to_obtain: Email info@yatmo.com or contact the reseller to receive a backend key.
  location: header
  name: LicenseKey (backend)
  type: http-header
- evidence: Every request made by an SDK carries the licence and three mobile headers. The SDK reads the app id from the running app (Bundle.main.bundleIdentifier on iOS, context.packageName on Android).
  header: X-Yatmo-App-Id
  how_to_obtain: Register your app ids in the Yatmo account (self‑service or via contact).
  location: header
  name: X-Yatmo-App-Id
  type: http-header
slug: yatmo-authentication
source_filename: yatmo-authentication.yml
source_heading: Authentication Profile
source_url: https://documentation.yatmo.com/license
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://documentation.yatmo.com/license\nsources:\n- https://documentation.yatmo.com/license\n- https://documentation.yatmo.com/mcp/auth\n- https://documentation.yatmo.com/mobile/app-ids\n- https://documentation.yatmo.com/api/auth\ndescription: Yatmo uses API‑key authentication via HTTP headers. No OAuth flows are defined.\nschemes:\n- type: http-header\n  name: LicenseKey (backend)\n  evidence: Every request to the Yatmo API carries your backend license key in an HTTP header.\n  location: header\n  header: LicenseKey\n  how_to_obtain: Email info@yatmo.com or contact the reseller to receive a backend key.\n- type: http-header\n  name: X-Yatmo-App-Id\n  evidence: Every request made by an SDK carries the licence and three mobile headers. The SDK reads the app id from the running app (Bundle.main.bundleIdentifier\n    on iOS, context.packageName on Android).\n  location: header\n \
  \ header: X-Yatmo-App-Id\n  how_to_obtain: Register your app ids in the Yatmo account (self‑service or via contact).\nnote: No OAuth2 flows, scopes, or token URLs are documented for Yatmo. 3 extracted row(s) were dropped because their quote was not on the page.\ndocs: https://documentation.yatmo.com/license\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yatmo/refs/heads/main/authentication/yatmo-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Real Estate
- LocationIntelligence
- MappingAPI
- POIData
---
