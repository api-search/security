---
anonymous_access: false
api_key_in: []
api_specs:
- filename: appalachian-regional-commission-research-api-openapi.yml
  format: yaml
  label: ARC Research and Data API
  slug: arc-research-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/openapi/appalachian-regional-commission-research-api-openapi.yml
- filename: appalachian-regional-commission-geospatial-api-openapi.yml
  format: yaml
  label: ARC Geospatial API
  slug: arc-geospatial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/openapi/appalachian-regional-commission-geospatial-api-openapi.yml
- filename: appalachian-regional-commission-programs-api-openapi.yml
  format: yaml
  label: ARC Programs API
  slug: arc-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/openapi/appalachian-regional-commission-programs-api-openapi.yml
- filename: appalachian-regional-commission-content-api-openapi.yml
  format: yaml
  label: ARC Content API
  slug: arc-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/openapi/appalachian-regional-commission-content-api-openapi.yml
- filename: appalachian-regional-commission-taxonomy-api-openapi.yml
  format: yaml
  label: ARC Taxonomy API
  slug: arc-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/openapi/appalachian-regional-commission-taxonomy-api-openapi.yml
- filename: appalachian-regional-commission-discovery-api-openapi.yml
  format: yaml
  label: ARC API Discovery
  slug: arc-api-discovery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/openapi/appalachian-regional-commission-discovery-api-openapi.yml
auth_types: []
description: The Appalachian Regional Commission runs no developer program, issues no API keys and operates no signup. Both of its machine-readable surfaces are open to anonymous callers, which is the normal posture for a federal-state commission publishing public-interest data. Authentication exists only on the write and administrative paths, and those are staff-facing.
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Appalachian Regional Commission Authentication
name_suffix: Authentication
oauth_flows: []
overview: Appalachian Regional Commission declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Appalachian Regional Commission
provider_slug: appalachian-regional-commission
scheme_count: 0
schemes: []
slug: appalachian-regional-commission-authentication
source_filename: appalachian-regional-commission-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Appalachian Regional Commission\nproviderId: appalachian-regional-commission\ngenerated: '2026-09-07'\nmethod: probed\nsource: >-\n  Live anonymous calls to https://www.arc.gov/wp-json/ and\n  https://services.arcgis.com/nkunl3y8FDxPkXDl/arcgis/rest/services on 2026-09-07, plus the RFC 8414\n  authorization-server metadata served at\n  https://arcgov.maps.arcgis.com/.well-known/oauth-authorization-server.\ndescription: >-\n  The Appalachian Regional Commission runs no developer program, issues no API keys and operates no\n  signup. Both of its machine-readable surfaces are open to anonymous callers, which is the normal\n  posture for a federal-state commission publishing public-interest data. Authentication exists only\n  on the write and administrative paths, and those are staff-facing.\nsummary:\n  public_read: anonymous\n  api_keys_issued: false\n  developer_signup: false\n  oauth_for_third_parties:\
  \ false\nsurfaces:\n  - name: ARC WordPress REST API\n    host: www.arc.gov\n    base: https://www.arc.gov/wp-json\n    anonymous_read: true\n    evidence: >-\n      GET /wp-json/wp/v2/posts, /pages, /media, /report, /map, /resource, /staff, /event,\n      /success_story, /investment_priority, /ldd, /search and every taxonomy route returned HTTP 200\n      with no credentials on 2026-09-07.\n    schemes:\n      - type: none\n        applies_to: the entire public GET surface documented in openapi/\n        note: No securityScheme is declared, because none is required.\n      - type: http\n        scheme: basic\n        applies_to: write methods (POST/PUT/PATCH/DELETE) advertised on the same routes\n        note: >-\n          WordPress authenticates writes with Application Passwords over HTTP Basic. ARC publishes no\n          process for obtaining one; these are staff credentials, not a public integration path. The\n          derived OpenAPI documents therefore describe the GET surface\
  \ only.\n    gated_routes_observed:\n      - path: /wp/v2/users\n        status: 401\n        code: rest_user_cannot_view\n      - path: /wp/v2/settings\n        status: 401\n        code: rest_forbidden\n      - path: /wp/v2/comments\n        status: 403\n        code: rest_comment_disabled\n        note: Commenting is switched off site-wide, so this is a configuration block rather than an auth wall.\n  - name: ARC Geospatial API (ArcGIS hosted feature services)\n    host: services.arcgis.com\n    base: https://services.arcgis.com/nkunl3y8FDxPkXDl/arcgis/rest\n    anonymous_read: true\n    evidence: >-\n      GET /services (108 services), GET /services/arc_counties/FeatureServer,\n      /FeatureServer/0 and /FeatureServer/0/query?returnCountOnly=true (423 features) all returned\n      HTTP 200 with no token on 2026-09-07.\n    schemes:\n      - type: none\n        applies_to: query and describe operations on the 108 public feature services\n      - type: oauth2\n        applies_to: ARC's\
  \ ArcGIS Online organization (staff and content management)\n        issuer: https://arcgov.maps.arcgis.com\n        authorization_endpoint: https://arcgov.maps.arcgis.com/sharing/rest/oauth2/authorize\n        token_endpoint: https://arcgov.maps.arcgis.com/sharing/rest/oauth2/token\n        grant_types:\n          - authorization_code\n          - implicit\n        pkce: S256\n        metadata_document: well-known/appalachian-regional-commission-oauth-authorization-server.json\n        note: >-\n          Discovered by probe, not by documentation. This is Esri's ArcGIS Online OAuth server scoped\n          to ARC's organization tenant; ARC does not document it or invite third-party clients to it,\n          and no scopes are advertised in the metadata. It is recorded because the document is real\n          and served from ARC's org host, not because ARC offers OAuth to developers.\nnot_found:\n  - api key issuance or a developer portal on arc.gov\n  - documented authentication reference\
  \ page\n  - mutual TLS, openIdConnect or signed-request schemes\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appalachian-regional-commission/refs/heads/main/authentication/appalachian-regional-commission-authentication.yml
summary_line: 0 schemes
tags:
- Appalachia
- Economic Development
- Federal-Government
- Geospatial
- Government
- Infrastructure
- Open Data
- Regional Development
- Workforce Development
---
