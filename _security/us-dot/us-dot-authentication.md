---
api_key_in:
- header
- query
api_specs:
- filename: us-dot-faa-aeronautic-product-release-api-openapi.yml
  format: yaml
  label: FAA Aeronautic Product Release API (APRA)
  slug: faa-aeronautic-product-release-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-faa-aeronautic-product-release-api-openapi.yml
- filename: us-dot-faa-air-carrier-prd-api-openapi.yml
  format: yaml
  label: FAA Air Carrier Pilot Records Database (PRD) API
  slug: faa-air-carrier-prd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-faa-air-carrier-prd-api-openapi.yml
- filename: us-dot-faa-safety-assurance-system-api-openapi.yml
  format: yaml
  label: FAA Safety Assurance System (SAS) API
  slug: faa-safety-assurance-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-faa-safety-assurance-system-api-openapi.yml
- filename: us-dot-its-jpo-ode-rest-api-openapi.yml
  format: yaml
  label: USDOT ITS JPO Operational Data Environment (ODE) REST API
  slug: its-jpo-ode-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-its-jpo-ode-rest-api-openapi.yml
- filename: us-dot-faa-airport-status-web-service-openapi.yml
  format: yaml
  label: U.S. Department of Transportation Airport Status Web Service
  slug: us-dot-faa-airport-status-web-service-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/openapi/us-dot-faa-airport-status-web-service-openapi.yml
auth_types:
- none
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Us Dot Authentication
name_suffix: Authentication
oauth_flows: []
overview: U.S. Department of Transportation secures its APIs with none and apiKey across 8 declared security schemes, as derived from its OpenAPI definitions.
provider_name: U.S. Department of Transportation
provider_slug: us-dot
scheme_count: 8
schemes:
- applies_to: us-dot:faa-safety-assurance-system-api
  in: header
  name: apiKey
  note: Declared as a securityScheme but NOT applied — the spec has no top-level or operation-level `security` block, so generated clients omit it and get a gateway 401.
  parameter: X-API-KEY
  sources:
  - openapi/us-dot-faa-safety-assurance-system-api-openapi.yml
  type: apiKey
- applies_to: us-dot:faa-safety-assurance-system-api
  in: header
  name: appId
  note: Required alongside X-API-KEY. Same non-application problem.
  parameter: X-APP-ID
  sources:
  - openapi/us-dot-faa-safety-assurance-system-api-openapi.yml
  type: apiKey
- applies_to: us-dot:faa-air-carrier-prd-api
  in: header
  name: clientIdHeader
  note: Declared as a REQUIRED header parameter on every operation, not as a securityScheme. Paired with client_secret. An OAuth-shaped credential pair with no OAuth protocol — no token endpoint, no expiry, no scopes, no refresh.
  parameter: client_id
  sources:
  - openapi/us-dot-faa-air-carrier-prd-api-openapi.yml
  type: apiKey
- applies_to: us-dot:faa-air-carrier-prd-api
  in: header
  name: clientSecretHeader
  parameter: client_secret
  sources:
  - openapi/us-dot-faa-air-carrier-prd-api-openapi.yml
  type: apiKey
- alternate:
    in: query
    parameter: $$app_token
  applies_to:
  - us-dot:dot-data-hub-soda-api
  - us-dot:bts-open-data-soda-api
  docs: https://dev.socrata.com/docs/app-tokens.html
  in: header
  name: socrataAppToken
  note: NOT authentication. An application token identifies the calling application so Socrata can apply a per-application throttle instead of the shared anonymous pool. Every read works without it. Issued self-serve at https://data.transportation.gov/profile/edit/developer_settings.
  optional: true
  parameter: X-App-Token
  type: apiKey
- applies_to: us-dot:fmcsa-qcmobile-api
  docs: https://mobile.fmcsa.dot.gov/QCDevsite/docs/apiAccess
  in: query
  name: fmcsaWebKey
  note: Free, self-serve — the only self-serve API credential in the department. Requires a Login.gov account to obtain. Login.gov is the federal OIDC identity provider, but it gates key ISSUANCE, not the API itself; FMCSA exposes no OIDC discovery document.
  parameter: webKey
  type: apiKey
- applies_to: us-dot:fra-safety-data-api
  docs: https://safetydata.fra.dot.gov/MasterWebService/FRASafetyDataAPIs.aspx
  name: fraWebServiceAccount
  note: A "web service account" requested by emailing RsisSupport@dot.gov. Two separate request types — one for the full Data Download service, one for the Lite API. Neither WSDL declares a WS-Security policy; the credential model is not published.
  scheme: unspecified
  type: http
- applies_to: us-dot:its-jpo-ode-rest-api
  name: odeOperatorDefined
  note: The ODE Swagger 2.0 document declares no securityDefinitions. Authentication is whatever the deploying operator puts in front of it. Given this API writes to physical roadside units, that absence is the finding.
  type: none
slug: us-dot-authentication
source_filename: us-dot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  openapi/us-dot-faa-safety-assurance-system-api-openapi.yml (securitySchemes),\n  openapi/us-dot-faa-air-carrier-prd-api-openapi.yml (header parameters),\n  https://api.faa.gov/s/, https://mobile.fmcsa.dot.gov/QCDevsite/,\n  https://safetydata.fra.dot.gov/MasterWebService/FRASafetyDataAPIs.aspx,\n  https://dev.socrata.com/docs/app-tokens.html, live probes 2026-07-28\nsummary:\n  types:\n  - none\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  detail: >-\n    U.S. DOT uses NO OAuth 2.0 and NO OpenID Connect on any API. Every credentialed\n    surface is a static key or key-pair sent in request headers. The majority of the\n    department's API surface area requires no credential at all. There is no departmental\n    identity layer for API consumers — Login.gov appears once, in front of FMCSA key\n    issuance, not in front of an API.\n  spec_gap: >-\n\
  \    Only ONE of the five harvested specs declares securitySchemes at all (the FAA SAS\n    API). The FAA PRD API sends its credentials as ordinary header PARAMETERS with no\n    securityScheme and no security requirement, which is why a mechanical derive over\n    securitySchemes alone misses it. Both are recorded below.\nanonymous_surfaces:\n- api: us-dot:faa-airport-status-web-service\n  verified: '2026-07-28'\n  evidence: 'GET https://external-api.faa.gov/asws/api/airport/status/JFK -> 200'\n- api: us-dot:faa-aeronautic-product-release-api\n  verified: '2026-07-28'\n  evidence: 'GET https://external-api.faa.gov/apra/nfdc/nasr/info -> 200'\n- api: us-dot:dot-data-hub-soda-api\n  verified: '2026-07-28'\n  note: Optional app token only; not authentication.\n- api: us-dot:bts-open-data-soda-api\n  verified: '2026-07-28'\n- api: us-dot:faa-data-catalog-ckan-api\n  verified: '2026-07-28'\n  evidence: 'GET https://catalog.data.faa.gov/api/3/action/package_list -> 200'\n- api: us-dot:nhtsa-vpic-api\n\
  \  verified: '2026-07-28'\n  evidence: 'GET https://vpic.nhtsa.dot.gov/api/vehicles/getallmakes?format=json -> 200, 12,306 makes'\n- api: us-dot:nhtsa-safety-api\n  verified: '2026-07-28'\n  evidence: 'GET https://api.nhtsa.gov/complaints/complaintsByVehicle?make=honda&model=accord&modelYear=2020 -> 200'\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  applies_to: us-dot:faa-safety-assurance-system-api\n  sources:\n  - openapi/us-dot-faa-safety-assurance-system-api-openapi.yml\n  note: >-\n    Declared as a securityScheme but NOT applied — the spec has no top-level or\n    operation-level `security` block, so generated clients omit it and get a gateway 401.\n- name: appId\n  type: apiKey\n  in: header\n  parameter: X-APP-ID\n  applies_to: us-dot:faa-safety-assurance-system-api\n  sources:\n  - openapi/us-dot-faa-safety-assurance-system-api-openapi.yml\n  note: Required alongside X-API-KEY. Same non-application problem.\n- name: clientIdHeader\n  type:\
  \ apiKey\n  in: header\n  parameter: client_id\n  applies_to: us-dot:faa-air-carrier-prd-api\n  sources:\n  - openapi/us-dot-faa-air-carrier-prd-api-openapi.yml\n  note: >-\n    Declared as a REQUIRED header parameter on every operation, not as a securityScheme.\n    Paired with client_secret. An OAuth-shaped credential pair with no OAuth protocol —\n    no token endpoint, no expiry, no scopes, no refresh.\n- name: clientSecretHeader\n  type: apiKey\n  in: header\n  parameter: client_secret\n  applies_to: us-dot:faa-air-carrier-prd-api\n  sources:\n  - openapi/us-dot-faa-air-carrier-prd-api-openapi.yml\n- name: socrataAppToken\n  type: apiKey\n  in: header\n  parameter: X-App-Token\n  alternate:\n    in: query\n    parameter: $$app_token\n  applies_to: [us-dot:dot-data-hub-soda-api, us-dot:bts-open-data-soda-api]\n  optional: true\n  docs: https://dev.socrata.com/docs/app-tokens.html\n  note: >-\n    NOT authentication. An application token identifies the calling application so\n    Socrata\
  \ can apply a per-application throttle instead of the shared anonymous pool.\n    Every read works without it. Issued self-serve at\n    https://data.transportation.gov/profile/edit/developer_settings.\n- name: fmcsaWebKey\n  type: apiKey\n  in: query\n  parameter: webKey\n  applies_to: us-dot:fmcsa-qcmobile-api\n  docs: https://mobile.fmcsa.dot.gov/QCDevsite/docs/apiAccess\n  note: >-\n    Free, self-serve — the only self-serve API credential in the department. Requires a\n    Login.gov account to obtain. Login.gov is the federal OIDC identity provider, but it\n    gates key ISSUANCE, not the API itself; FMCSA exposes no OIDC discovery document.\n- name: fraWebServiceAccount\n  type: http\n  scheme: unspecified\n  applies_to: us-dot:fra-safety-data-api\n  docs: https://safetydata.fra.dot.gov/MasterWebService/FRASafetyDataAPIs.aspx\n  note: >-\n    A \"web service account\" requested by emailing RsisSupport@dot.gov. Two separate\n    request types — one for the full Data Download service,\
  \ one for the Lite API. Neither\n    WSDL declares a WS-Security policy; the credential model is not published.\n- name: odeOperatorDefined\n  type: none\n  applies_to: us-dot:its-jpo-ode-rest-api\n  note: >-\n    The ODE Swagger 2.0 document declares no securityDefinitions. Authentication is\n    whatever the deploying operator puts in front of it. Given this API writes to physical\n    roadside units, that absence is the finding.\ncredential_issuance:\n- portal: https://api.faa.gov/s/\n  covers: [us-dot:faa-air-carrier-prd-api, us-dot:faa-safety-assurance-system-api]\n  self_serve: false\n  gate: FAA operator accreditation (14 CFR Part 121/135/125/91K/Air Tour/Public Aircraft/91 Corporate for PRD)\n  guide: https://www.faa.gov/regulationspolicies/pilotrecordsdatabase/air-carrier-api-discover-learn-get-access\n- portal: https://mobile.fmcsa.dot.gov/QCDevsite/\n  covers: [us-dot:fmcsa-qcmobile-api]\n  self_serve: true\n  identity: Login.gov\n- portal: 'mailto:RsisSupport@dot.gov'\n  covers:\
  \ [us-dot:fra-safety-data-api]\n  self_serve: false\n- portal: https://data.transportation.gov/profile/edit/developer_settings\n  covers: [us-dot:dot-data-hub-soda-api, us-dot:bts-open-data-soda-api]\n  self_serve: true\n  optional: true\noauth:\n  supported: false\n  evidence:\n  - '/.well-known/oauth-authorization-server -> 404 on every DOT, BTS and FAA host probed 2026-07-28'\n  - '/.well-known/openid-configuration -> 404 on every host probed'\n  - No OpenAPI declares an oauth2 securityScheme\n  consequence: >-\n    No scopes/ artifact is emitted for this provider. There is no scope surface to\n    describe — key-auth providers have no OAuth scope model, and forcing an empty\n    artifact would be misleading.\ntransport:\n  tls_minimum_observed: TLSv1.2\n  detail: See security/us-dot-domain-security.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-dot/refs/heads/main/authentication/us-dot-authentication.yml
summary_line: none/apiKey · 8 schemes
tags:
- Travel
- United States
- Aviation
- Airlines
- Airports
- Government
- Regulator
- Distribution
- Aviation Consumer Protection
- Open Data
- Transportation
- Safety
- Statistics
- Automotive
- Rail
---
