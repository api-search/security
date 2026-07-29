---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: derived
name: Transport Canada Authentication
name_suffix: Authentication
oauth_flows: []
overview: Transport Canada secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Transport Canada
provider_slug: transport-canada
scheme_count: 0
schemes: []
slug: transport-canada-authentication
source_filename: transport-canada-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: derived\nsource: >-\n  Derived from the machine-readable service descriptors harvested into\n  capabilities/ and from the anonymous HTTP probes recorded in review.yml\n  (2026-07-28). Transport Canada publishes no OpenAPI, so there are no\n  securitySchemes to aggregate; this profile records the auth model that the\n  live endpoints actually enforce.\ndocs: https://open.canada.ca/en/access-our-application-programming-interface-api\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    All three Transport Canada public interfaces are genuinely unauthenticated.\n    Every probe in review.yml was issued from a clean anonymous client and\n    returned HTTP 200. There is no API key, no OAuth client registration, no\n    signed request, and no click-through terms gate. \"Self-serve\" here means\n    no credential exists, not \"register for a free key\".\nschemes: []\napis:\n  - aid: transport-canada:transport-canada-vehicle-recalls-database-api\n\
  \    baseURL: https://data.tc.gc.ca/v1.3/api/eng/vehicle-recall-database\n    authentication: none\n    evidence: >-\n      GET /v1.3/api/eng/vehicle-recall-database/recall/recall-number/2024001?format=json\n      returned 200 with a full record and no credential (review.yml probes).\n  - aid: transport-canada:transport-canada-canadian-airports-arcgis-rest-api\n    baseURL: >-\n      https://maps-cartes.services.geo.ca/server_serveur/rest/services/TC/canadian_airports_w_air_navigation_services_en/MapServer\n    authentication: none\n    evidence: >-\n      MapServer?f=json and layer 0 /query both returned 200 anonymously. The\n      ArcGIS service descriptor declares no token endpoint and no secured\n      capability (capabilities/transport-canada-airports-arcgis-mapserver.json).\n  - aid: transport-canada:transport-canada-canadian-airports-wms\n    baseURL: >-\n      https://maps-cartes.services.geo.ca/server_serveur/services/TC/canadian_airports_w_air_navigation_services_en/MapServer/WMSServer\n\
  \    authentication: none\n    evidence: >-\n      WMS_Capabilities 1.3.0 carries an empty <Fees/> element and an\n      <AccessConstraints> of \"Open Government Licence - Canada\" — the OGC\n      encoding of unrestricted access\n      (capabilities/transport-canada-airports-wms-capabilities.xml).\nauthorization:\n  model: none\n  scopes: none\n  note: >-\n    There is no scope, role or permission surface. Access control is exercised\n    upstream of the API by deciding which datasets get published at all; the\n    published surface is fully open under the Open Government Licence - Canada.\ngated_surfaces:\n  - name: Drone Management Portal\n    url: https://tc.canada.ca/en/aviation/drone-safety/drone-management-portal\n    authentication: GCKey / Sign-In Partner account (interactive only)\n    note: >-\n      Regulatory account service for RPAS registration and pilot certificates.\n      Human sign-in only; no public API, no OAuth client registration, and no\n      documented machine\
  \ interface.\n  - name: Canadian Civil Aircraft Register (CCARCS)\n    url: https://wwwapps.tc.gc.ca/saf-sec-sur/2/ccarcs-riacc/RchSimp.aspx\n    authentication: none\n    note: >-\n      Unauthenticated but non-programmatic — an ASP.NET search form capped at\n      1000 results with no API and no bulk download.\nlicense: https://open.canada.ca/en/open-government-licence-canada\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-canada/refs/heads/main/authentication/transport-canada-authentication.yml
summary_line: none · 0 schemes
tags:
- Travel
- Canada
- Aviation
- Regulator
- Government
- Airports
- Aircraft Registry
- Aviation Safety
- Drones
- Open Data
- Transportation
---
