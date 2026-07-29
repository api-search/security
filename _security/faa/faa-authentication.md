---
api_key_in:
- header
api_specs:
- filename: faa-airport-status-web-service-openapi.yml
  format: yaml
  label: FAA Airport Status Web Service (ASWS)
  slug: faa-airport-status-web-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faa/refs/heads/main/openapi/faa-airport-status-web-service-openapi.yml
- filename: faa-aeronautic-product-release-api-openapi.yml
  format: yaml
  label: FAA Aeronautic Product Release API (APRA)
  slug: faa-aeronautic-product-release-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faa/refs/heads/main/openapi/faa-aeronautic-product-release-api-openapi.yml
- filename: faa-air-carrier-prd-api-openapi.yml
  format: yaml
  label: FAA Air Carrier PRD API
  slug: faa-air-carrier-prd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faa/refs/heads/main/openapi/faa-air-carrier-prd-api-openapi.yml
- filename: faa-safety-assurance-system-api-openapi.yml
  format: yaml
  label: FAA Safety Assurance System (SAS) API
  slug: faa-safety-assurance-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/faa/refs/heads/main/openapi/faa-safety-assurance-system-api-openapi.yml
auth_types:
- none
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Faa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Federal Aviation Administration secures its APIs with none and apiKey across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Federal Aviation Administration
provider_slug: faa
scheme_count: 5
schemes:
- applies_to:
  - FAA Airport Status Web Service (ASWS)
  - FAA Aeronautic Product Release API (APRA)
  - FAA NAS Status airport status information feed
  - FAA Temporary Flight Restriction (TFR) list API
  - FAA NMS North Atlantic Track NOTAM feed
  - FAA NMS system metrics feed
  - FAA Data Catalog (CKAN)
  - FAA AIS and UDDS ArcGIS Open Data hubs
  - Releasable aircraft registry bulk ZIP
  evidence: Neither the ASWS nor the APRA OpenAPI declares components.securitySchemes, both declare a Creative Commons Zero (CC0) licence, and the FAA's own Gravitee plan for each is KEY_LESS. Unauthenticated HTTP 200 verified on both, and on the TFR, NAS status and NMS feeds, on 2026-07-28.
  name: none
  type: none
- applied: false
  applied_note: DEFINED in components.securitySchemes but never APPLIED — the SAS spec declares no root-level and no operation-level `security`, so tooling reads the operation as unauthenticated. Flagged in overlays/faa-safety-assurance-system-api-overlay.yaml.
  applies_to:
  - FAA Safety Assurance System (SAS) API
  in: header
  name: apiKey
  parameter: X-API-KEY
  sources:
  - openapi/faa-safety-assurance-system-api-openapi.yml
  type: apiKey
- applied: false
  applies_to:
  - FAA Safety Assurance System (SAS) API
  in: header
  name: appId
  note: Paired with X-API-KEY. Same never-applied problem.
  parameter: X-APP-ID
  sources:
  - openapi/faa-safety-assurance-system-api-openapi.yml
  type: apiKey
- applies_to:
  - FAA Air Carrier PRD API
  - FAA NOTAM API
  declared_as: required header parameters on every operation, NOT a securityScheme
  evidence: 'All eight PRD operations declare both as `required: true` header parameters. An unauthenticated GET to https://external-api.faa.gov/notamapi/v1/notams returned HTTP 401 {"message":"Unauthorized","http_status_code":401} on 2026-07-28.'
  in: header
  name: client_id + client_secret
  parameter: client_id, client_secret
  sources:
  - openapi/faa-air-carrier-prd-api-openapi.yml
  type: apiKey
  weakness: A client SECRET carried as a plain request header with no token exchange, no expiry and no rotation policy — and modelled as a parameter, so generated clients and API tooling do not recognise the API as authenticated at all. This guards the most sensitive data in the FAA estate (pilot employment, training, drug/alcohol and disciplinary records).
- evidence: https://apim-api.apic4e.faa.gov/portal/environments/DEFAULT/configuration reports the gateway apikeyHeader as X-Gravitee-Api-Key.
  in: header
  name: X-Gravitee-Api-Key
  note: The API-management gateway's own key header. Appears in no FAA OpenAPI, so a developer working from the specs alone would not know it exists.
  parameter: X-Gravitee-Api-Key
  sources:
  - portal configuration endpoint
  type: apiKey
slug: faa-authentication
source_filename: faa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  openapi/*.yml in this repo, plus the FAA Gravitee developer-portal REST API\n  (https://apim-api.apic4e.faa.gov/portal/environments/DEFAULT/configuration and\n  /apis/{id}/plans), https://www.faa.gov/data, https://nms.aim.faa.gov/ and\n  https://www.faa.gov/air_traffic/technology/swim/products/get_connected — all\n  fetched 2026-07-28\ndocs: https://www.faa.gov/data\nupgrades: >-\n  Upgrades the 2026-07-28 derived pass, which saw only the two apiKey schemes in the\n  SAS spec. The FAA's real credential model is wider than its securitySchemes: two\n  APIs need no credential at all, one declares its credential as ordinary header\n  PARAMETERS rather than a scheme, and the gateway itself has a key header that\n  appears in no spec.\nsummary:\n  types: [none, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  oidc: false\n  mtls: false\n  key_issuance: self-serve account and application creation, then\
  \ MANUAL approval per API\n  headline: >-\n    No OAuth 2.0 and no OpenID Connect anywhere in the FAA public API estate. Every\n    credentialed FAA API is a static shared secret carried in a request header, with\n    no token exchange, no expiry, no rotation policy and no scopes. Two APIs — the\n    two most useful ones — need no credential at all.\nschemes:\n- name: none\n  type: none\n  applies_to:\n  - FAA Airport Status Web Service (ASWS)\n  - FAA Aeronautic Product Release API (APRA)\n  - FAA NAS Status airport status information feed\n  - FAA Temporary Flight Restriction (TFR) list API\n  - FAA NMS North Atlantic Track NOTAM feed\n  - FAA NMS system metrics feed\n  - FAA Data Catalog (CKAN)\n  - FAA AIS and UDDS ArcGIS Open Data hubs\n  - Releasable aircraft registry bulk ZIP\n  evidence: >-\n    Neither the ASWS nor the APRA OpenAPI declares components.securitySchemes, both\n    declare a Creative Commons Zero (CC0) licence, and the FAA's own Gravitee plan\n    for each is KEY_LESS.\
  \ Unauthenticated HTTP 200 verified on both, and on the TFR,\n    NAS status and NMS feeds, on 2026-07-28.\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources: [openapi/faa-safety-assurance-system-api-openapi.yml]\n  applies_to: [FAA Safety Assurance System (SAS) API]\n  applied: false\n  applied_note: >-\n    DEFINED in components.securitySchemes but never APPLIED — the SAS spec declares no\n    root-level and no operation-level `security`, so tooling reads the operation as\n    unauthenticated. Flagged in overlays/faa-safety-assurance-system-api-overlay.yaml.\n- name: appId\n  type: apiKey\n  in: header\n  parameter: X-APP-ID\n  sources: [openapi/faa-safety-assurance-system-api-openapi.yml]\n  applies_to: [FAA Safety Assurance System (SAS) API]\n  applied: false\n  note: Paired with X-API-KEY. Same never-applied problem.\n- name: client_id + client_secret\n  type: apiKey\n  in: header\n  parameter: client_id, client_secret\n  declared_as: required header\
  \ parameters on every operation, NOT a securityScheme\n  sources: [openapi/faa-air-carrier-prd-api-openapi.yml]\n  applies_to:\n  - FAA Air Carrier PRD API\n  - FAA NOTAM API\n  evidence: >-\n    All eight PRD operations declare both as `required: true` header parameters. An\n    unauthenticated GET to https://external-api.faa.gov/notamapi/v1/notams returned\n    HTTP 401 {\"message\":\"Unauthorized\",\"http_status_code\":401} on 2026-07-28.\n  weakness: >-\n    A client SECRET carried as a plain request header with no token exchange, no\n    expiry and no rotation policy — and modelled as a parameter, so generated clients\n    and API tooling do not recognise the API as authenticated at all. This guards the\n    most sensitive data in the FAA estate (pilot employment, training, drug/alcohol\n    and disciplinary records).\n- name: X-Gravitee-Api-Key\n  type: apiKey\n  in: header\n  parameter: X-Gravitee-Api-Key\n  sources: [portal configuration endpoint]\n  evidence: >-\n    https://apim-api.apic4e.faa.gov/portal/environments/DEFAULT/configuration\
  \ reports\n    the gateway apikeyHeader as X-Gravitee-Api-Key.\n  note: >-\n    The API-management gateway's own key header. Appears in no FAA OpenAPI, so a\n    developer working from the specs alone would not know it exists.\nonboarding:\n  portal: https://api.faa.gov/\n  portal_actual: https://portal.apic4e.faa.gov/ (301 from api.faa.gov)\n  software: Gravitee.io APIM Developer Portal\n  self_serve: true\n  evidence: >-\n    Portal configuration reports userCreation.enabled=true and\n    applicationCreation.enabled=true. The FAA Data Portal says verbatim: \"Developers\n    can easily integrate FAA dataset into software applications thanks to the FAA's\n    Application Programming Interfaces (APIs). Get started by creating an API key\".\n  approval: >-\n    Every API_KEY plan in the portal is validation MANUAL — an account is self-serve\n    but a subscription is approved by the FAA API owner. The Air Carrier PRD plan\n    additionally sets comment_required, so a justification must be\
  \ supplied.\n  out_of_band:\n  - api: FAA NOTAM Management Service (NMS)\n    method: email request to notams@faa.gov\n    source: https://nms.aim.faa.gov/\n    verbatim: 'Please contact us at notams@faa.gov to request access to the new NMS-API.'\n  - api: SWIM / SWIM Cloud Distribution Service\n    method: executed FAA SWIM agreement via the SWIFT Portal\n    source: https://portal.swim.faa.gov/\n  - api: SWIM CDM, TFMS Request/Reply, TFMS International Data Provider\n    method: email request to Data-To-Industry@faa.gov, reviewed in accordance with FAA policy\n  - api: LAANC\n    method: only through an FAA-Approved UAS Service Supplier, never directly\neligibility_gates:\n- api: FAA Air Carrier PRD API\n  gate: regulatory\n  verbatim: >-\n    \"Access is restricted to operators under Part 121, 135, 125, 91K, Air Tour, Public\n    Aircraft, or 91 Corporate. Requests for access from any other public or private\n    entities will not be authorized.\"\n  source: FAA Gravitee portal catalog\
  \ record\nscopes:\n  present: false\n  note: >-\n    No OAuth means no scope surface. This repo deliberately carries no scopes/\n    artifact — see conventions/faa-conventions.yml.\ndiscovery:\n  oauth_authorization_server: 404 on every FAA host probed\n  openid_configuration: 404 on every FAA host probed\n  source: well-known/faa-well-known.yml\ngaps:\n- No OAuth 2.0 / OIDC anywhere, so no delegated access and no consent model.\n- No scopes, so no least-privilege credential for any FAA API.\n- No documented key rotation, expiry or revocation policy.\n- The PRD credential is modelled as a parameter, not a security scheme.\n- The SAS security schemes are defined but never applied.\n- The gateway key header appears in no published spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/faa/refs/heads/main/authentication/faa-authentication.yml
summary_line: none/apiKey · 5 schemes
tags:
- Travel
- United States
- Aviation
- Airports
- Government
- Regulator
- Open Data
- Airspace
- Drones
- Aeronautical Information
---
