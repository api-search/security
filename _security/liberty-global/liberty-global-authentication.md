---
api_key_in: []
api_specs:
- filename: liberty-global-appstore-metadata-service-openapi.yml
  format: yaml
  label: AppStore Metadata Service API
  slug: appstore-metadata-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberty-global/refs/heads/main/openapi/liberty-global-appstore-metadata-service-openapi.yml
- filename: liberty-global-appstore-bundle-service-openapi.yml
  format: yaml
  label: AppStore Bundle Service API
  slug: appstore-bundle-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberty-global/refs/heads/main/openapi/liberty-global-appstore-bundle-service-openapi.yml
- filename: liberty-global-appstore-caching-service-openapi.yml
  format: yaml
  label: AppStore Caching Service API
  slug: appstore-caching-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liberty-global/refs/heads/main/openapi/liberty-global-appstore-caching-service-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Liberty Global Authentication
name_suffix: Authentication
oauth_flows: []
overview: Liberty Global secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Liberty Global
provider_slug: liberty-global
scheme_count: 2
schemes:
- applies_to: Every write and maintainer-scoped operation — createMaintainer, getMaintainer, replaceMaintainer, deleteMaintainer, listMaintainerApplications, createMaintainerApplication, getMaintainerApplication, replaceMaintainerApplication, deleteMaintainerApplication
  declared_in_spec: false
  documented_example: 'Authorization: Basic <base64 of the as3 dev user>'
  enforced_by: The AS3 Proxy, an Nginx server in front of ASMS that exposes the metadata management methods and authorizes each maintainer to their own applications. Not enforced by the ASMS service itself.
  name: as3-basic
  perspective: Maintainer (AS3)
  scheme: basic
  source: https://github.com/LibertyGlobal/appstore-metadata-service#request-samples
  type: http
- applies_to: 'Read-only discovery operations: listApplications, getApplicationDetails'
  declared_in_spec: false
  documented_example: 'Authorization: Basic <base64 of the stb dev user>'
  enforced_by: The ASMS Proxy, a separate Nginx server that limits the method set exposed to set-top-box devices to fetch-only. The README states this component "should be providing unique authentication/authorization capabilities in future versions of the ASMS initiative" — i.e. the STB-side auth model is explicitly acknowledged as unfinished.
  name: stb-basic
  perspective: STB
  scheme: basic
  source: https://github.com/LibertyGlobal/appstore-metadata-service#request-samples
  type: http
slug: liberty-global-authentication
source_filename: liberty-global-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/*.yml (derived — none found) + provider README (searched)\ndocs: https://github.com/LibertyGlobal/appstore-metadata-service/blob/master/README.md\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  declared_in_openapi: false\n  documented_in_readme: true\nnote: >-\n  0-working/derive-authentication.py returned zero schemes: none of the three\n  harvested OpenAPI documents declares a `securitySchemes` block, and none\n  applies `security` at the document or operation level. The auth model is\n  nevertheless real and documented — it lives in the AppStore Metadata Service\n  README rather than in the specification. That is the finding: an\n  authenticated API whose contract does not describe its own authentication.\nschemes:\n- name: as3-basic\n  type: http\n  scheme: basic\n  perspective: Maintainer (AS3)\n  applies_to: >-\n    Every write and maintainer-scoped operation — createMaintainer,\n\
  \    getMaintainer, replaceMaintainer, deleteMaintainer,\n    listMaintainerApplications, createMaintainerApplication,\n    getMaintainerApplication, replaceMaintainerApplication,\n    deleteMaintainerApplication\n  enforced_by: >-\n    The AS3 Proxy, an Nginx server in front of ASMS that exposes the metadata\n    management methods and authorizes each maintainer to their own\n    applications. Not enforced by the ASMS service itself.\n  documented_example: \"Authorization: Basic <base64 of the as3 dev user>\"\n  source: https://github.com/LibertyGlobal/appstore-metadata-service#request-samples\n  declared_in_spec: false\n- name: stb-basic\n  type: http\n  scheme: basic\n  perspective: STB\n  applies_to: 'Read-only discovery operations: listApplications, getApplicationDetails'\n  enforced_by: >-\n    The ASMS Proxy, a separate Nginx server that limits the method set exposed\n    to set-top-box devices to fetch-only. The README states this component\n    \"should be providing unique authentication/authorization\
  \ capabilities in\n    future versions of the ASMS initiative\" — i.e. the STB-side auth model is\n    explicitly acknowledged as unfinished.\n  documented_example: \"Authorization: Basic <base64 of the stb dev user>\"\n  source: https://github.com/LibertyGlobal/appstore-metadata-service#request-samples\n  declared_in_spec: false\nunauthenticated_surfaces:\n- api: openapi/liberty-global-appstore-bundle-service-openapi.yml\n  note: >-\n    The AppStore Bundle Service specification declares no securitySchemes and\n    the README shows no Authorization header on any call. It is an internal\n    service reached from the caching layer, not a public endpoint.\n- api: openapi/liberty-global-appstore-caching-service-openapi.yml\n  note: >-\n    Same. The caching service is an Nginx proxy in front of the bundle service;\n    no auth is declared or documented.\ngroup_level:\n  camara_apis:\n    auth_model: not published by Liberty Global\n    note: >-\n      The CAMARA network APIs the group sells\
  \ (SIM Swap, Number Verification,\n      KYC Age Verify, KYC Tenure) are onboarded through the operating joint\n      ventures — Virgin Media O2 and VodafoneZiggo — not through the parent.\n      No OIDC discovery document, no CIBA endpoint and no client-credentials\n      flow is published on any libertyglobal.com host; see\n      well-known/liberty-global-well-known.yml. CAMARA's own security profile\n      builds on OIDC/CIBA, but Liberty Global publishes nothing that would let\n      a developer authenticate.\n    ciba: false\n    oidc_discovery: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liberty-global/refs/heads/main/authentication/liberty-global-authentication.yml
summary_line: http · 2 schemes
tags:
- Telecommunications
- United Kingdom
- Broadband
- Fixed Broadband
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- 5G
- Europe
- Set-Top Box
- RDK
---
