---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Fair Housing And Equal Opportunity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fair Housing and Equal Opportunity declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Fair Housing and Equal Opportunity
provider_slug: fair-housing-and-equal-opportunity
scheme_count: 0
schemes: []
slug: fair-housing-and-equal-opportunity-authentication
source_filename: fair-housing-and-equal-opportunity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  Live unauthenticated calls on 2026-09-07 against every FHEO baseURL, plus the\n  response headers those calls returned. derive-authentication.py found no\n  securitySchemes because there is no OpenAPI to read.\nprovider: Fair Housing and Equal Opportunity\nproviderId: fair-housing-and-equal-opportunity\nsummary: >-\n  Every FHEO surface in this record is anonymously readable. No key, no token,\n  no account, no registration. An unauthenticated GET against the FHAP grantee\n  layer's /query endpoint returned HTTP 200 with feature data, and the service\n  advertises capabilities \"Query,Extract\" only — there is no write surface to\n  authenticate against.\nschemes: []\nscheme_count: 0\nposture:\n  anonymous_read: true\n  registration_required: false\n  api_key_required: false\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  write_surface: false\nevidence:\n  - url: https://services.arcgis.com/VTyQ9soqVukalItT/arcgis/rest/services/Fair_Housing_Assistance_Program_Grantees/FeatureServer/0/query?where=1%3D1&outFields=FHAP_NAME,STATE&returnGeometry=false&resultRecordCount=2&f=json\n\
  \    method: GET\n    credentials_sent: none\n    http_status: 200\n    result: features returned\n  - url: https://services.arcgis.com/VTyQ9soqVukalItT/arcgis/rest/services/Fair_Housing_Assistance_Program_Grantees/FeatureServer?f=pjson\n    method: GET\n    credentials_sent: none\n    http_status: 200\n    result: 'capabilities: \"Query,Extract\"'\n  - url: https://egis.hud.gov/arcgis/rest/services/affht/AffhtMapService/MapServer?f=pjson\n    method: GET\n    credentials_sent: none\n    http_status: 200\n    result: service metadata returned\noptional_credential:\n  supported: true\n  note: >-\n    The ArcGIS Online services vary on X-Esri-Authorization (the response\n    carries `vary: X-Esri-Authorization`) and accept an Authorization or\n    X-Esri-Authorization header, so an ArcGIS Online token CAN be presented.\n    Presenting one is never required for these public layers; it only moves the\n    request onto the caller's own ArcGIS organisation quota. This is Esri\n    platform behaviour,\
  \ not an FHEO-published auth scheme, which is why no\n    scheme is listed above.\ndiscovery:\n  well_known_openid_configuration: 404\n  well_known_oauth_authorization_server: 404\n  note: >-\n    Probed on www.hud.gov, hud.gov, www.huduser.gov, egis.hud.gov and\n    hudgis-hud.opendata.arcgis.com. See\n    well-known/fair-housing-and-equal-opportunity-well-known.yml.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fair-housing-and-equal-opportunity/refs/heads/main/authentication/fair-housing-and-equal-opportunity-authentication.yml
summary_line: 0 schemes
tags:
- AFFH
- ArcGIS
- Equal Opportunity
- Fair Housing
- Federal-Government
- Geospatial
- Housing
- HUD
- Open Data
---
