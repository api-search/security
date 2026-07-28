---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Manitoba Hydro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Manitoba Hydro secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Manitoba Hydro
provider_slug: manitoba-hydro
scheme_count: 1
schemes:
- applies_to:
  - manitoba-hydro:manitoba-hydro-current-power-outages
  - manitoba-hydro:manitoba-hydro-planned-power-outages
  - manitoba-hydro:manitoba-hydro-arcgis-server-reference-data
  - manitoba-hydro:manitoba-hydro-hydrological-data
  evidence:
  - note: Anonymous attribute query returned features with no token parameter.
    status: 200
    url: https://services2.arcgis.com/QoeQkfdOG126FqSi/arcgis/rest/services/Manitoba_Hydro_Current_Power_Outages/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=3&f=json
  - note: Anonymous attribute query returned features with no token parameter.
    status: 200
    url: https://services2.arcgis.com/QoeQkfdOG126FqSi/arcgis/rest/services/Manitoba_Hydro_Planned_Power_Outages/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=3&f=json
  - note: Anonymous query against Manitoba Hydro's own ArcGIS Server host. The host root at https://maps.hydro.mb.ca/ returns HTTP 403; only the /arcgis/rest/services tree is readable.
    status: 200
    url: https://maps.hydro.mb.ca/arcgis/rest/services/ReferenceData/MH_AdminBoundaries/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=3&f=json
  - note: Anonymous WFS 2.0.0 GetCapabilities.
    status: 200
    url: https://dservices2.arcgis.com/QoeQkfdOG126FqSi/arcgis/services/Manitoba_Hydro_Current_Power_Outages_WFS/WFSServer?service=wfs&request=getcapabilities
  - note: Anonymous, but an F5 web application firewall on www.hydro.mb.ca intermittently answers HTTP 200 with a "Request Rejected" HTML body when the request does not look like a browser. Sending a browser User-Agent and a Referer of https://www.hydro.mb.ca/hydrologicalData/static/ gets through reliably. This is a bot-mitigation filter, not authentication.
    status: 200
    url: https://www.hydro.mb.ca/hydrologicalData/static/data/tsdata.json
  name: none
  type: none
slug: manitoba-hydro-authentication
source_filename: manitoba-hydro-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  live anonymous HTTPS probes of every apis.yml surface on 2026-07-27, plus\n  review.yml authModel section\ndocs: null\ndocs_note: >-\n  Manitoba Hydro publishes no developer authentication documentation of any\n  kind. There is no developer portal, no key issuance page, and no token\n  endpoint. This profile was established by probing, not by reading a doc.\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  anonymous: true\n  registration_required: false\n  credentials_issued: false\nmodel: >-\n  Anonymous by default on every published surface. Every Manitoba Hydro API\n  surface catalogued in apis.yml answered an unauthenticated request with no\n  key, token, referer allow-list entry, or registration. There is nothing to\n  obtain and nothing to rotate. The absence of authentication here is not a\n  security posture decision about an API programme — it is the by-product of a\n  GIS team sharing ArcGIS\
  \ Online items publicly and a hydrology team publishing\n  static JSON behind a public web application.\nschemes:\n- name: none\n  type: none\n  applies_to:\n  - manitoba-hydro:manitoba-hydro-current-power-outages\n  - manitoba-hydro:manitoba-hydro-planned-power-outages\n  - manitoba-hydro:manitoba-hydro-arcgis-server-reference-data\n  - manitoba-hydro:manitoba-hydro-hydrological-data\n  evidence:\n  - url: https://services2.arcgis.com/QoeQkfdOG126FqSi/arcgis/rest/services/Manitoba_Hydro_Current_Power_Outages/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=3&f=json\n    status: 200\n    note: Anonymous attribute query returned features with no token parameter.\n  - url: https://services2.arcgis.com/QoeQkfdOG126FqSi/arcgis/rest/services/Manitoba_Hydro_Planned_Power_Outages/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=3&f=json\n    status: 200\n    note: Anonymous attribute query returned features with no token\
  \ parameter.\n  - url: https://maps.hydro.mb.ca/arcgis/rest/services/ReferenceData/MH_AdminBoundaries/FeatureServer/0/query?where=1%3D1&outFields=*&returnGeometry=false&resultRecordCount=3&f=json\n    status: 200\n    note: >-\n      Anonymous query against Manitoba Hydro's own ArcGIS Server host. The host\n      root at https://maps.hydro.mb.ca/ returns HTTP 403; only the\n      /arcgis/rest/services tree is readable.\n  - url: https://dservices2.arcgis.com/QoeQkfdOG126FqSi/arcgis/services/Manitoba_Hydro_Current_Power_Outages_WFS/WFSServer?service=wfs&request=getcapabilities\n    status: 200\n    note: Anonymous WFS 2.0.0 GetCapabilities.\n  - url: https://www.hydro.mb.ca/hydrologicalData/static/data/tsdata.json\n    status: 200\n    note: >-\n      Anonymous, but an F5 web application firewall on www.hydro.mb.ca\n      intermittently answers HTTP 200 with a \"Request Rejected\" HTML body when\n      the request does not look like a browser. Sending a browser User-Agent and\n      a Referer\
  \ of https://www.hydro.mb.ca/hydrologicalData/static/ gets through\n      reliably. This is a bot-mitigation filter, not authentication.\ntoken_endpoints: []\ndiscovery:\n  openid_configuration: null\n  oauth_authorization_server: null\n  probed:\n  - {url: 'https://www.hydro.mb.ca/.well-known/openid-configuration', status: 404}\n  - {url: 'https://www.hydro.mb.ca/.well-known/oauth-authorization-server', status: 404}\n  - {url: 'https://account.hydro.mb.ca/.well-known/openid-configuration', status: 404}\n  - {url: 'https://account.hydro.mb.ca/.well-known/oauth-authorization-server', status: 404}\nconsumer_authentication:\n  scheme: username-password\n  url: https://account.hydro.mb.ca/Portal\n  platform: Smart Energy Water — Smart Customer Mobile (Android package com.sew.manitoba)\n  third_party_delegation: none\n  note: >-\n    The only place a Manitoba Hydro customer's own usage or billing data lives is\n    behind an interactive login at account.hydro.mb.ca. There is no OAuth\n    authorization\
  \ server, no consent screen, no delegated-access programme, and\n    no accredited-recipient regime — Manitoba has no consumer energy data\n    mandate and Manitoba Hydro has no advanced metering infrastructure producing\n    interval data in the first place. The portal's vendor backend is visible at\n    https://account.hydro.mb.ca/API/ (\"SCM Service API\", HTTP 200) but lists no\n    operations and its help page returns HTTP 403; it is a first-party SaaS\n    backend, not a third-party API.\nagent_guidance: >-\n  An agent can call every surface in this repo directly over HTTPS with no\n  credential handling at all. Send a realistic User-Agent, and for\n  www.hydro.mb.ca also send a Referer matching the hydrological application, or\n  the WAF will return an HTTP 200 \"Request Rejected\" page that is not JSON. Do\n  not attempt to reach consumer usage data — no API path to it exists.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manitoba-hydro/refs/heads/main/authentication/manitoba-hydro-authentication.yml
summary_line: none · 1 scheme
tags:
- Energy
- Canada
- Utilities
- Electricity
- Gas
- Hydroelectric
- Grid
- Outage Data
- Open Data
- Crown Corporation
---
