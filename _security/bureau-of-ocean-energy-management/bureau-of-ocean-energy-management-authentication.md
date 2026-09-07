---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Bureau Of Ocean Energy Management Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bureau of Ocean Energy Management declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Bureau of Ocean Energy Management
provider_slug: bureau-of-ocean-energy-management
scheme_count: 0
schemes: []
slug: bureau-of-ocean-energy-management-authentication
source_filename: bureau-of-ocean-energy-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  live anonymous probes 2026-09-05 of https://gis.boem.gov/server/rest/services,\n  the OGC WMS/WFS endpoints under /server/services/, https://hub.marinecadastre.gov/data.json\n  and https://esp-boem.hub.arcgis.com/data.json\nnote: |\n  BOEM's public data surfaces require NO authentication. Every probe below was made anonymously\n  with no key, no token and no cookie, and every one returned data. There is no developer\n  portal, no signup, no API key issuance and no OAuth authorization server anywhere on the\n  estate — /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n  returned 404 on all six hosts probed (see well-known/).\n\n  The ArcGIS Server directory does advertise a login and a token endpoint\n  (https://gis.boem.gov/server/rest/login and https://gis.boem.gov/server/tokens/). These are\n  the stock Esri ArcGIS Server administrative surfaces, not a consumer credential path — they\n  exist\
  \ to let BOEM staff publish services, and nothing in BOEM's own documentation offers a\n  reader an account. They are recorded here so a later round does not read them as a public\n  auth tier.\nschemes: []\nsurfaces:\n  - name: BOEM ArcGIS REST Services\n    base: https://gis.boem.gov/server/rest/services\n    auth: none\n    evidence: >-\n      GET /server/rest/services?f=json returned HTTP 200 with the folder list, and\n      /BOEM_BSEE/ATL_Layers/MapServer/0/query?where=1=1&returnCountOnly=true&f=json returned\n      {\"count\":975} — both anonymous\n  - name: BOEM OGC WMS / WFS\n    base: https://gis.boem.gov/server/services\n    auth: none\n    evidence: >-\n      eleven GetCapabilities documents fetched anonymously at HTTP 200; saved verbatim to openapi/\n  - name: MarineCadastre.gov DCAT catalog\n    base: https://hub.marinecadastre.gov\n    auth: none\n    evidence: GET /data.json returned HTTP 200, 275 datasets, anonymous\n  - name: ESPIS ArcGIS Hub\n    base: https://esp-boem.hub.arcgis.com\n\
  \    auth: none\n    evidence: GET /data.json returned HTTP 200, 11 datasets, anonymous\nadministrative_surfaces:\n  - url: https://gis.boem.gov/server/rest/login\n    kind: ArcGIS Server administrative sign-in\n    public: false\n  - url: https://gis.boem.gov/server/tokens/\n    kind: ArcGIS Server token service\n    public: false\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-ocean-energy-management/refs/heads/main/authentication/bureau-of-ocean-energy-management-authentication.yml
summary_line: 0 schemes
tags:
- Energy
- Federal-Government
- Marine
- Oceans
- GIS
- Offshore
- Environmental
---
