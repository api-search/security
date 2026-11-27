---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Statistik Austria Authentication
name_suffix: Authentication
oauth_flows: []
overview: Statistik Austria declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Statistik Austria
provider_slug: statistik-at
scheme_count: 3
schemes:
- api: statistik-at:statcube-open-data-api
  description: STATcube REST API requires an API key, available to all STATcube subscribers and displayed under the STATcube account preferences. An unauthenticated GET /info returns 401 {"errorType":"AUTHENTICATION"}.
  evidence: https://statcubeapi.statistik.at/statistik.at/ext/statcube/rest/v1/info (HTTP 401, probed 2026-11-11)
  type: apiKey
- api: statistik-at:open-government-data
  description: Open Government Data datasets and JSON metadata are public with no authentication.
  evidence: https://data.statistik.gv.at/ogd/json?dataset=OGD_veste309_Veste309_1 (HTTP 200, probed 2026-11-11)
  type: none
- api: statistik-at:geodata-ogc
  description: WMS/WFS GetCapabilities answer anonymously.
  evidence: https://www.statistik.at/gs-open/GEODATA/ows?service=WFS&request=GetCapabilities (HTTP 200, probed 2026-11-11)
  type: none
slug: statistik-at-authentication
source_filename: statistik-at-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Statistik Austria authentication\ngenerated: '2026-11-11'\nmethod: searched\nsource: https://statistikat.github.io/STATcubeR/articles/sc_key.html\ndocs: https://www.statistik.at/en/databases/statcube-statistical-database/subscription-access\nschemes:\n- api: statistik-at:statcube-open-data-api\n  type: apiKey\n  description: STATcube REST API requires an API key, available to all STATcube subscribers and displayed under the STATcube account preferences. An unauthenticated GET /info returns 401 {\"errorType\":\"AUTHENTICATION\"}.\n  evidence: https://statcubeapi.statistik.at/statistik.at/ext/statcube/rest/v1/info (HTTP 401, probed 2026-11-11)\n- api: statistik-at:open-government-data\n  type: none\n  description: Open Government Data datasets and JSON metadata are public with no authentication.\n  evidence: https://data.statistik.gv.at/ogd/json?dataset=OGD_veste309_Veste309_1 (HTTP 200, probed 2026-11-11)\n- api: statistik-at:geodata-ogc\n  type: none\n  description: WMS/WFS\
  \ GetCapabilities answer anonymously.\n  evidence: https://www.statistik.at/gs-open/GEODATA/ows?service=WFS&request=GetCapabilities (HTTP 200, probed 2026-11-11)\n"
source_yaml_url: https://artifacts.apis.io/statistik-at/authentication/statistik-at-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Official Statistics
- Government
- Open Data
- Austria
- Statistics
- Geospatial
- OGC
---
