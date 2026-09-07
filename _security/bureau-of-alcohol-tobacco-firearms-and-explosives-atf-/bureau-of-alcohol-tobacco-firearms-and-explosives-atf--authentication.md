---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bureau-of-alcohol-tobacco-firearms-and-explosives-atf--eregulations-openapi.yml
  format: yaml
  label: ATF eRegulations API
  slug: atf-eregulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-alcohol-tobacco-firearms-and-explosives-atf-/refs/heads/main/openapi/bureau-of-alcohol-tobacco-firearms-and-explosives-atf--eregulations-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Bureau Of Alcohol Tobacco Firearms And Explosives Atf  Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bureau of Alcohol, Tobacco, Firearms and Explosives (ATF) declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Bureau of Alcohol, Tobacco, Firearms and Explosives (ATF)
provider_slug: bureau-of-alcohol-tobacco-firearms-and-explosives-atf-
scheme_count: 0
schemes: []
slug: bureau-of-alcohol-tobacco-firearms-and-explosives-atf--authentication
source_filename: bureau-of-alcohol-tobacco-firearms-and-explosives-atf--authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nprovider: Bureau of Alcohol, Tobacco, Firearms and Explosives (ATF)\nproviderId: bureau-of-alcohol-tobacco-firearms-and-explosives-atf-\nsource: >-\n  Live anonymous requests on 2026-09-05 to every public ATF API endpoint found by\n  contract discovery. No credential of any kind was presented and every request\n  succeeded.\nsummary: >-\n  There is no authentication. ATF's entire public API surface — the eRegulations\n  JSON API and both ArcGIS feature services — answers unauthenticated GET requests\n  with data. No API key, no OAuth client, no signup, no registration, no rate-limit\n  token. For an agent this is the simplest possible posture: no onboarding step\n  exists to complete.\nschemes: []\nposture:\n  anonymous: true\n  registration_required: false\n  key_issuance: none\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  signing: none\nevidence:\n  - surface: ATF eRegulations API\n    url: https://regulations.atf.gov/api/regulation\n\
  \    status: 200\n    detail: 200 application/json with no Authorization header sent.\n  - surface: ATF eRegulations search\n    url: https://regulations.atf.gov/api/search?q=firearm\n    status: 200\n    detail: 200 application/json, 1,596 total_hits, anonymous.\n  - surface: Federal Firearm Licensees locations (ArcGIS Feature Service)\n    url: https://services6.arcgis.com/PrP5ZtrES07DmVmv/arcgis/rest/services/Federal_Firearm_Licensees_locations/FeatureServer/0/query?where=1%3D1&returnCountOnly=true&f=json\n    status: 200\n    detail: 200 {\"count\":77514}, anonymous. Item `access` is \"public\" in ArcGIS Online.\n  - surface: ATF Office Locations (ArcGIS Feature Service)\n    url: https://services6.arcgis.com/PrP5ZtrES07DmVmv/arcgis/rest/services/ATF_Office_Locations/FeatureServer/0/query?where=1%3D1&returnCountOnly=true&f=json\n    status: 200\n    detail: 200 {\"count\":537}, anonymous.\n  - surface: /.well-known/oauth-authorization-server\n    url: https://www.atf.gov/.well-known/oauth-authorization-server\n\
  \    status: 403\n    detail: >-\n      No authorization-server metadata anywhere. The 403 is an Akamai edge refusal\n      of our crawler, not an ATF answer; the same path on regulations.atf.gov\n      returns the app's HTML shell, which is equally not a discovery document.\ngated_surfaces:\n  - name: ATF eForms\n    url: https://eforms.atf.gov/\n    note: >-\n      Licensee-facing form filing behind a Login.gov account. It is a web\n      application, not a documented API; no machine interface is published.\n  - name: eTrace / National Tracing Center\n    url: https://www.atf.gov/firearms/etrace-internet-based-firearms-tracing-and-analysis\n    note: >-\n      Restricted to credentialed law-enforcement agencies. Not a public API and\n      not scored as one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-alcohol-tobacco-firearms-and-explosives-atf-/refs/heads/main/authentication/bureau-of-alcohol-tobacco-firearms-and-explosives-atf--authentication.yml
summary_line: 0 schemes
tags:
- Alcohol
- Explosives
- Federal-Government
- Firearms
- Geospatial
- Law Enforcement
- Open Data
- Public Safety
- Regulations
- Tobacco
---
