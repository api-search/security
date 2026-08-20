---
api_key_in: []
api_specs:
- filename: geoinsight-ogc-api-dggs-openapi.yml
  format: yaml
  label: OGC API - DGGS
  slug: ogc-api-dggs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/openapi/geoinsight-ogc-api-dggs-openapi.yml
auth_types: []
description: 'GeoInsight''s published OpenAPI declares NO components.securitySchemes and NO top-level security requirement, so the machine-readable contract says nothing about authentication. The credential model is documented only in the README of the first-party PyPI package: a GeoInsight Personal Token (GPT) and an API Private Key (APK), obtained by creating an account on the dashboard, then set with api.set_access_token(_gpt=''GPT'', _apk=''APK''). The package depends on auth0-python, which indicates the token issuance path runs through Auth0. Neither the wire format (header name, scheme, encoding) nor the token lifetime is published anywhere machine- or human-readable that could be found.'
kind: authentication
layout: security
method: searched
name: Geoinsight Authentication
name_suffix: Authentication
oauth_flows: []
overview: GeoInsight declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: GeoInsight
provider_slug: geoinsight
scheme_count: 0
schemes: []
slug: geoinsight-authentication
source_filename: geoinsight-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-20'\nmethod: searched\nsource: https://pypi.org/project/geoinsight/\nspec_source: openapi/geoinsight-ogc-api-dggs-openapi.yml\ndocs: https://pypi.org/project/geoinsight/\nname: GeoInsight Authentication Profile\ndescription: >-\n  GeoInsight's published OpenAPI declares NO components.securitySchemes and NO top-level security\n  requirement, so the machine-readable contract says nothing about authentication. The credential model is\n  documented only in the README of the first-party PyPI package: a GeoInsight Personal Token (GPT) and an\n  API Private Key (APK), obtained by creating an account on the dashboard, then set with\n  api.set_access_token(_gpt='GPT', _apk='APK'). The package depends on auth0-python, which indicates the\n  token issuance path runs through Auth0. Neither the wire format (header name, scheme, encoding) nor the\n  token lifetime is published anywhere machine- or human-readable that could be found.\nsummary:\n  types: []\n  api_key_in:\
  \ []\n  oauth2_flows: []\n  spec_declares_security: false\n  note: >-\n    The empty lists are the finding, not a gap in this artifact. The spec genuinely declares no\n    securityScheme.\nschemes: []\ndocumented_credentials:\n  - name: GeoInsight Personal Token (GPT)\n    abbreviation: GPT\n    issued_by: https://dashboard.geoinsight.ai\n    documented_in: https://pypi.org/project/geoinsight/\n    wire_format: unpublished\n    note: >-\n      Set client-side via geoinsight.api().set_access_token(_gpt=..., _apk=...). The header or query\n      parameter the SDK puts it on is not documented and there is no source repository to read it from.\n  - name: API Private Key (APK)\n    abbreviation: APK\n    issued_by: https://dashboard.geoinsight.ai\n    documented_in: https://pypi.org/project/geoinsight/\n    wire_format: unpublished\nidentity_provider:\n  vendor: Auth0\n  evidence: >-\n    The official PyPI package geoinsight 0.8.1 declares auth0-python>=4.4.2 as a runtime dependency.\n  confidence:\
  \ medium\n  note: Inferred from the dependency list, not from a GeoInsight statement. No OIDC discovery document is served.\nobserved_behaviour:\n  anonymous_reads: true\n  evidence:\n    - {url: 'https://api.geoinsight.ai/', status: 200, note: Landing page document returned without credentials}\n    - {url: 'https://api.geoinsight.ai/collections?f=json', status: 200, note: 22 collections returned without credentials}\n    - {url: 'https://api.geoinsight.ai/dggs?f=json', status: 200, note: DGGRS registry returned without credentials}\n    - {url: 'https://api.geoinsight.ai/api?f=json', status: 200, note: OpenAPI document returned without credentials}\n  note: >-\n    Every operation reachable during this pass answered anonymously. No 401 or 403 was observed on any\n    path. It is not possible to tell from the outside whether the GPT/APK pair gates a subset of\n    collections, raises quota, or is simply not yet enforced on this deployment.\ncredential_path_status:\n  reachable: false\n\
  \  url: https://dashboard.geoinsight.ai\n  http_status: 404\n  note: >-\n    The dashboard the package README names as the place to obtain a GPT and APK returns an nginx\n    \"default backend - 404\" on every path behind a self-signed Kubernetes ingress certificate. A\n    developer following the official install instructions today cannot obtain credentials.\ngaps:\n  - No securitySchemes in the OpenAPI, so no generated client can authenticate from the contract.\n  - No documented header name or scheme for the GPT/APK pair.\n  - No token lifetime, rotation or revocation policy published.\n  - No OIDC or OAuth discovery document on any host (see well-known/geoinsight-well-known.yml).\n  - The documented credential-issuance host is unreachable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geoinsight/refs/heads/main/authentication/geoinsight-authentication.yml
summary_line: 0 schemes
tags:
- Geospatial
- DGGS
- Discrete Global Grid System
- Earth Observation
- Remote Sensing
- Spatial Data
- GIS
- Artificial Intelligence
- Machine-Learning
- Analysis-ready data
- Spatial Tokens
- Sentinel-2
- Copernicus
- OGC
- STAC
- GeoParquet
- H3
---
