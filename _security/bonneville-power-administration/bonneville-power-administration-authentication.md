---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bonneville-power-administration-customers-api-openapi.yml
  format: yaml
  label: Bonneville Power Administration Customers API
  slug: bonneville-power-administration-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonneville-power-administration/refs/heads/main/openapi/bonneville-power-administration-customers-api-openapi.yml
- filename: bonneville-power-administration-hydrology-api-openapi.yml
  format: yaml
  label: Bonneville Power Administration Hydrology API
  slug: bonneville-power-administration-hydrology-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonneville-power-administration/refs/heads/main/openapi/bonneville-power-administration-hydrology-api-openapi.yml
- filename: bonneville-power-administration-right-of-way-api-openapi.yml
  format: yaml
  label: Bonneville Power Administration Right of Way API
  slug: bonneville-power-administration-right-of-way-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonneville-power-administration/refs/heads/main/openapi/bonneville-power-administration-right-of-way-api-openapi.yml
- filename: bonneville-power-administration-service-area-api-openapi.yml
  format: yaml
  label: Bonneville Power Administration Service Area API
  slug: bonneville-power-administration-service-area-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonneville-power-administration/refs/heads/main/openapi/bonneville-power-administration-service-area-api-openapi.yml
- filename: bonneville-power-administration-transmission-api-openapi.yml
  format: yaml
  label: Bonneville Power Administration Transmission API
  slug: bonneville-power-administration-transmission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonneville-power-administration/refs/heads/main/openapi/bonneville-power-administration-transmission-api-openapi.yml
- filename: bonneville-power-administration-data-search-api-openapi.yml
  format: yaml
  label: Bonneville Power Administration Data Search API
  slug: bonneville-power-administration-data-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bonneville-power-administration/refs/heads/main/openapi/bonneville-power-administration-data-search-api-openapi.yml
auth_types: []
description: 'Authentication profile for the BPA public API surface. There is no credential to obtain: BPA''s published ArcGIS Online layers are shared publicly and answer anonymous GET requests with HTTP 200, and the transmission.bpa.gov operational data files are static public downloads. No sign-up, no API key, no OAuth.'
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Bonneville Power Administration Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bonneville Power Administration declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Bonneville Power Administration
provider_slug: bonneville-power-administration
scheme_count: 0
schemes: []
slug: bonneville-power-administration-authentication
source_filename: bonneville-power-administration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  live anonymous requests to\n  https://services3.arcgis.com/Iz3chmSt4P7oOoZy/arcgis/rest/services/BPA_ServiceArea/FeatureServer/0/query\n  plus openapi/_original/bonneville-power-administration-openapi.yml\nprovider: Bonneville Power Administration\nproviderId: bonneville-power-administration\ndocs: https://data-bpagis.hub.arcgis.com\ndescription: >-\n  Authentication profile for the BPA public API surface. There is no credential to\n  obtain: BPA's published ArcGIS Online layers are shared publicly and answer\n  anonymous GET requests with HTTP 200, and the transmission.bpa.gov operational\n  data files are static public downloads. No sign-up, no API key, no OAuth.\nsummary:\n  schemes: 0\n  anonymous_access: true\n  registration_required: false\n  verdict: public-anonymous\nschemes: []\nsurfaces:\n- name: BPA GIS Data Hub — ArcGIS REST FeatureServer\n  base: https://services3.arcgis.com/Iz3chmSt4P7oOoZy/arcgis/rest\n \
  \ auth: none\n  evidence:\n    url: https://services3.arcgis.com/Iz3chmSt4P7oOoZy/arcgis/rest/services/BPA_ServiceArea/FeatureServer/0/query?where=1%3D1&outFields=*&f=json\n    http_status: 200\n    fetched: '2026-09-06'\n    note: >-\n      Returned a full FeatureSet with no credential. The service /info document\n      reports authInfo.isTokenBasedSecurity true and a tokenServicesUrl at\n      www.arcgis.com, which is the Esri platform's token service for PRIVATE items\n      in the tenant; the BPA layers registered in this repo are shared publicly and\n      do not require it.\n  optional_credential:\n    type: arcgis-token\n    header: X-Esri-Authorization\n    query_param: token\n    token_service: https://www.arcgis.com/sharing/rest/generateToken\n    applies_to: private items in the BPA ArcGIS Online tenant, not the public layers here\n    note: >-\n      Platform-level Esri mechanism, not a BPA-issued credential. Recorded because the\n      service /info document advertises it;\
  \ no BPA public layer in this repo needs it.\n- name: BPA Balancing Authority load and VER generation data\n  base: https://transmission.bpa.gov/business/operations/wind/\n  auth: none\n  evidence:\n    url: https://transmission.bpa.gov/business/operations/wind/baltwg.txt\n    http_status: 200\n    fetched: '2026-09-06'\n    note: Plain-text 5-minute-interval feed served anonymously, no credential.\n- name: BPA OASIS node (NAESB WEQ-002 transmission service)\n  base: http://www.oasis.oati.com/bpat/\n  auth: gated\n  evidence:\n    url: http://www.oasis.oati.com/bpat/index.html\n    http_status: 0\n    fetched: '2026-09-06'\n    note: >-\n      DNS resolves (174.141.249.8 / 216.234.82.8) but the connection times out from a\n      general-purpose client. OATI OASIS nodes are registered-participant surfaces;\n      credentials are issued by OATI to transmission customers, not published by BPA.\n      Not probed further and NOT registered as a callable API in this record.\nnotes:\n- No API\
  \ key, OAuth client, or account registration exists for any BPA public data surface.\n- >-\n  Because there is no credential to rotate, scope, or leak, the OAuthScopes and Sandbox\n  artifacts are not applicable for this provider and are deliberately absent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bonneville-power-administration/refs/heads/main/authentication/bonneville-power-administration-authentication.yml
summary_line: 0 schemes
tags:
- Energy
- Federal-Government
- GIS
- Hydroelectric
- Pacific Northwest
- Power
- Transmission
- Wind
---
