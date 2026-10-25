---
anonymous_access: true
api_key_in: []
api_specs:
- filename: bureau-of-ocean-energy-management-catalog-api-openapi.yml
  format: yaml
  label: Bureau of Ocean Energy Management Catalog API
  slug: bureau-of-ocean-energy-management-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-ocean-energy-management/refs/heads/main/openapi/bureau-of-ocean-energy-management-catalog-api-openapi.yml
- filename: bureau-of-ocean-energy-management-collection-api-openapi.yml
  format: yaml
  label: Bureau of Ocean Energy Management Collection API
  slug: bureau-of-ocean-energy-management-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-ocean-energy-management/refs/heads/main/openapi/bureau-of-ocean-energy-management-collection-api-openapi.yml
- filename: bureau-of-ocean-energy-management-geoservice-beta-api-openapi.yml
  format: yaml
  label: Bureau of Ocean Energy Management Geoservice Beta API
  slug: bureau-of-ocean-energy-management-geoservice-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-ocean-energy-management/refs/heads/main/openapi/bureau-of-ocean-energy-management-geoservice-beta-api-openapi.yml
- filename: bureau-of-ocean-energy-management-ogcitem-api-openapi.yml
  format: yaml
  label: Bureau of Ocean Energy Management Ogc Item API
  slug: bureau-of-ocean-energy-management-ogcitem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-ocean-energy-management/refs/heads/main/openapi/bureau-of-ocean-energy-management-ogcitem-api-openapi.yml
- filename: bureau-of-ocean-energy-management-ogcitemaggregation-api-openapi.yml
  format: yaml
  label: Bureau of Ocean Energy Management Ogc Item Aggregation API
  slug: bureau-of-ocean-energy-management-ogcitemaggregation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-ocean-energy-management/refs/heads/main/openapi/bureau-of-ocean-energy-management-ogcitemaggregation-api-openapi.yml
- filename: bureau-of-ocean-energy-management-ogcroot-api-openapi.yml
  format: yaml
  label: Bureau of Ocean Energy Management Ogc Root API
  slug: bureau-of-ocean-energy-management-ogcroot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-ocean-energy-management/refs/heads/main/openapi/bureau-of-ocean-energy-management-ogcroot-api-openapi.yml
- filename: bureau-of-ocean-energy-management-ogcrootconformance-api-openapi.yml
  format: yaml
  label: Bureau of Ocean Energy Management Ogc Root Conformance API
  slug: bureau-of-ocean-energy-management-ogcrootconformance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-ocean-energy-management/refs/heads/main/openapi/bureau-of-ocean-energy-management-ogcrootconformance-api-openapi.yml
- filename: bureau-of-ocean-energy-management-queryable-api-openapi.yml
  format: yaml
  label: Bureau of Ocean Energy Management Queryable API
  slug: bureau-of-ocean-energy-management-queryable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-ocean-energy-management/refs/heads/main/openapi/bureau-of-ocean-energy-management-queryable-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Bureau Of Ocean Energy Management Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bureau of Ocean Energy Management declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bureau of Ocean Energy Management
provider_slug: bureau-of-ocean-energy-management
scheme_count: 1
schemes:
- description: All public BOEM data surfaces (ArcGIS REST, OGC WMS/WFS, DCAT data.json, Marine Cadastre Hub Search API) answered anonymous requests with data; no credential is issued to the public.
  evidence: https://gis.boem.gov/server/rest/services?f=json (200 anonymous); https://hub.marinecadastre.gov/api/search/v1/conformance (200 anonymous, 2026-10-20)
  name: anonymous
  type: none
slug: bureau-of-ocean-energy-management-authentication
source_filename: bureau-of-ocean-energy-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live anonymous probes 2026-09-05 of https://gis.boem.gov/server/rest/services,\n  the OGC WMS/WFS endpoints under /server/services/, https://hub.marinecadastre.gov/data.json\n  and https://esp-boem.hub.arcgis.com/data.json\nnote: 'BOEM''s public data surfaces require NO authentication. Every probe below was\n  made anonymously\n\n  with no key, no token and no cookie, and every one returned data. There is no developer\n\n  portal, no signup, no API key issuance and no OAuth authorization server anywhere\n  on the\n\n  estate — /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n\n  returned 404 on all six hosts probed (see well-known/).\n\n\n  The ArcGIS Server directory does advertise a login and a token endpoint\n\n  (https://gis.boem.gov/server/rest/login and https://gis.boem.gov/server/tokens/).\n  These are\n\n  the stock Esri ArcGIS Server administrative surfaces, not a consumer credential\n \
  \ path — they\n\n  exist to let BOEM staff publish services, and nothing in BOEM''s own documentation\n  offers a\n\n  reader an account. They are recorded here so a later round does not read them as\n  a public\n\n  auth tier.\n\n  '\nschemes:\n- type: none\n  name: anonymous\n  description: All public BOEM data surfaces (ArcGIS REST, OGC WMS/WFS, DCAT data.json,\n    Marine Cadastre Hub Search API) answered anonymous requests with data; no credential\n    is issued to the public.\n  evidence: https://gis.boem.gov/server/rest/services?f=json (200 anonymous); https://hub.marinecadastre.gov/api/search/v1/conformance\n    (200 anonymous, 2026-10-20)\nsurfaces:\n- name: BOEM ArcGIS REST Services\n  base: https://gis.boem.gov/server/rest/services\n  auth: none\n  evidence: GET /server/rest/services?f=json returned HTTP 200 with the folder list,\n    and /BOEM_BSEE/ATL_Layers/MapServer/0/query?where=1=1&returnCountOnly=true&f=json\n    returned {\"count\":975} — both anonymous\n- name: BOEM\
  \ OGC WMS / WFS\n  base: https://gis.boem.gov/server/services\n  auth: none\n  evidence: eleven GetCapabilities documents fetched anonymously at HTTP 200; saved\n    verbatim to openapi/\n- name: MarineCadastre.gov DCAT catalog\n  base: https://hub.marinecadastre.gov\n  auth: none\n  evidence: GET /data.json returned HTTP 200, 275 datasets, anonymous\n- name: ESPIS ArcGIS Hub\n  base: https://esp-boem.hub.arcgis.com\n  auth: none\n  evidence: GET /data.json returned HTTP 200, 11 datasets, anonymous\nadministrative_surfaces:\n- url: https://gis.boem.gov/server/rest/login\n  kind: ArcGIS Server administrative sign-in\n  public: false\n- url: https://gis.boem.gov/server/tokens/\n  kind: ArcGIS Server token service\n  public: false\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-ocean-energy-management/refs/heads/main/authentication/bureau-of-ocean-energy-management-authentication.yml
summary_line: 1 scheme
tags:
- Energy
- Federal Government
- Marine
- Ocean
- GIS
- Offshore
- Environmental
---
