---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: probed
name: Essential Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Essential Energy secures its APIs with none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Essential Energy
provider_slug: essential-energy
scheme_count: 2
schemes:
- description: All 100 public ArcGIS REST FeatureServers under org 3o0vFs4fJRsuYuBO answer unauthenticated requests. No Authorization header, no api key parameter, no cookie and no referrer restriction was required for any verified call.
  name: anonymous
  sources:
  - arcgis/essential-energy-arcgis-services-catalog.json
  - examples/essential-energy-examples.yml
  type: none
  verified:
  - request: GET https://services-ap1.arcgis.com/3o0vFs4fJRsuYuBO/arcgis/rest/services?f=json
    status: 200
  - request: GET https://services-ap1.arcgis.com/3o0vFs4fJRsuYuBO/arcgis/rest/services/HostingCapacity_Substation_GEN/FeatureServer/1/query?where=1%3D1&outFields=*&resultRecordCount=2&f=json
    status: 200
  - note: returned {"count":144569}
    request: GET https://services-ap1.arcgis.com/3o0vFs4fJRsuYuBO/arcgis/rest/services/Substation/FeatureServer/0/query?where=1%3D1&returnCountOnly=true&f=json
    status: 200
- description: The hosting platform (Esri ArcGIS Online) advertises token-based security for content that is NOT shared publicly. This is an Esri platform mechanism bound to an ArcGIS Online named user, not an Essential Energy developer credential — Essential Energy issues no accounts against it and none of the public layers require it.
  is_token_based_security: true
  name: arcgis-token
  owning_system_url: https://www.arcgis.com
  owning_tenant: 3o0vFs4fJRsuYuBO
  platform: Esri ArcGIS Online
  portal_token_service: https://www.arcgis.com/sharing/rest/generateToken
  sources:
  - arcgis/essential-energy-arcgis-rest-info.json
  token_service: https://www.arcgis.com/sharing/generateToken
  type: token
slug: essential-energy-authentication
source_filename: essential-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  https://services-ap1.arcgis.com/3o0vFs4fJRsuYuBO/arcgis/rest/info?f=json and\n  https://essentialenergy.maps.arcgis.com/sharing/rest/info?f=json (both HTTP 200,\n  anonymous, 2026-07-27), plus repeated anonymous query calls against the published\n  FeatureServers.\ndocs: null\nsummary:\n  types:\n  - none\n  api_key_in: []\n  oauth2_flows: []\n  headline: >-\n    The public Essential Energy API surface requires NO authentication. Every published\n    FeatureServer answers anonymous HTTPS GET. Esri token-based security exists on the\n    hosting platform for non-public content, but no Essential Energy credential, key,\n    signup or accreditation is issued to developers.\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n    All 100 public ArcGIS REST FeatureServers under org 3o0vFs4fJRsuYuBO answer\n    unauthenticated requests. No Authorization header, no api key parameter, no cookie\n    and no referrer restriction\
  \ was required for any verified call.\n  verified:\n  - request: >-\n      GET https://services-ap1.arcgis.com/3o0vFs4fJRsuYuBO/arcgis/rest/services?f=json\n    status: 200\n  - request: >-\n      GET https://services-ap1.arcgis.com/3o0vFs4fJRsuYuBO/arcgis/rest/services/HostingCapacity_Substation_GEN/FeatureServer/1/query?where=1%3D1&outFields=*&resultRecordCount=2&f=json\n    status: 200\n  - request: >-\n      GET https://services-ap1.arcgis.com/3o0vFs4fJRsuYuBO/arcgis/rest/services/Substation/FeatureServer/0/query?where=1%3D1&returnCountOnly=true&f=json\n    status: 200\n    note: returned {\"count\":144569}\n  sources:\n  - arcgis/essential-energy-arcgis-services-catalog.json\n  - examples/essential-energy-examples.yml\n- name: arcgis-token\n  type: token\n  description: >-\n    The hosting platform (Esri ArcGIS Online) advertises token-based security for\n    content that is NOT shared publicly. This is an Esri platform mechanism bound to an\n    ArcGIS Online named user, not an Essential\
  \ Energy developer credential — Essential\n    Energy issues no accounts against it and none of the public layers require it.\n  platform: Esri ArcGIS Online\n  token_service: https://www.arcgis.com/sharing/generateToken\n  portal_token_service: https://www.arcgis.com/sharing/rest/generateToken\n  is_token_based_security: true\n  owning_system_url: https://www.arcgis.com\n  owning_tenant: 3o0vFs4fJRsuYuBO\n  sources:\n  - arcgis/essential-energy-arcgis-rest-info.json\nnot_present:\n  api_key: >-\n    No API key is issued or required. developer., developers., api. and docs.\n    essentialenergy.com.au do not resolve (NXDOMAIN, verified 2026-07-27), so there is\n    no key-issuing developer portal.\n  oauth2: >-\n    No OAuth 2.0 authorization or token endpoint is published by Essential Energy.\n    /.well-known/oauth-authorization-server returns 403 (Cloudflare) on www. and 404 on\n    dapr. and engage. hosts.\n  openid_connect: >-\n    /.well-known/openid-configuration returns no document\
  \ on any Essential Energy host.\n  mutual_tls: >-\n    No mTLS profile is published. No client-certificate challenge was observed on any\n    verified call.\n  cdr_accreditation: >-\n    The Australian Consumer Data Right accreditation model does NOT apply. Essential\n    Energy is a distribution network service provider and is absent from the public CDR\n    energy data-holder brand register (see review.yml mandate.statusEvidence).\ngated_surfaces:\n- name: Network Information Portal\n  description: >-\n    The ordering of formal network data packages (pole data, network routes) for\n    Accredited Service Providers, electrical contractors, councils and emergency\n    services runs through a request/order workflow behind Esri/ArcGIS Online identity.\n    That is a customer/partner login, not a published developer auth scheme, and it\n    exposes no documented API.\n  url: https://engage.essentialenergy.com.au/access-to-network-data\nobservations:\n- >-\n    Service metadata for Suitable_Poles_2026\
  \ advertises capabilities \"Query,Update,Editing\"\n    while every other sampled service advertises \"Query\" or \"Query,Extract\". This is\n    recorded verbatim from the published service descriptor; no write operation was\n    attempted. Read-only consumers should treat the surface as query-only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/essential-energy/refs/heads/main/authentication/essential-energy-authentication.yml
summary_line: none · 2 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Network Distributor
- Open Data
- GIS
- DER
- Hosting Capacity
- EV Charging
- Renewables
- New South Wales
---
