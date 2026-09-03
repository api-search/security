---
api_key_in: []
api_specs:
- filename: texas-a-m-university-geoservices-geocoding-openapi.yml
  format: yaml
  label: Texas A&M GeoServices Geocoding API
  slug: geoservices-geocode
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-a-m-university/refs/heads/main/openapi/texas-a-m-university-geoservices-geocoding-openapi.yml
- filename: texas-a-m-university-aggiemap-dining-openapi.yml
  format: yaml
  label: Aggie Map Dining Locations API
  slug: aggiemap-dining
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-a-m-university/refs/heads/main/openapi/texas-a-m-university-aggiemap-dining-openapi.yml
- filename: texas-a-m-university-campus-micromobility-openapi.yml
  format: yaml
  label: Campus Micromobility Vehicle Positions API
  slug: campus-micromobility
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-a-m-university/refs/heads/main/openapi/texas-a-m-university-campus-micromobility-openapi.yml
- filename: texas-a-m-university-identity-federation-openapi.yml
  format: yaml
  label: Texas A&M Shibboleth Identity Provider Metadata
  slug: identity-federation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-a-m-university/refs/heads/main/openapi/texas-a-m-university-identity-federation-openapi.yml
auth_types: []
description: 'How authentication works across the Texas A&M University surfaces this repository records. The estate splits three ways: a small set of open, unauthenticated campus and geospatial feeds; one key-gated but freely self-serve research API; and an enterprise tier at the Texas A&M University System that cannot be reached at all without a sponsored account.'
kind: authentication
layout: security
method: probed
name: Texas A M University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Texas A&M University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Texas A&M University
provider_slug: texas-a-m-university
scheme_count: 0
schemes: []
slug: texas-a-m-university-authentication
source_filename: texas-a-m-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# x-method: derived\n# Authored by API Evangelist from live probes and published documentation on 2026-09-01.\n# The in-file `method:` records HOW the evidence was obtained (probed / derived);\n# this line records WHO WROTE THE FILE, in the provenance manifest's vocabulary.\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live anonymous probes on 2026-09-01 of geoservices.tamu.edu, api.aggiemap.tamu.edu,\n  veoride.geoservices.tamu.edu, gis.it.tamu.edu, idp.tamu.edu, mdq.incommon.org,\n  oaktrust.library.tamu.edu, catalog.tamu.edu and api-doc.sea.system.tamus.edu, plus the published\n  access policy at https://it.tamus.edu/uinmanager/api/.\ndescription: >-\n  How authentication works across the Texas A&M University surfaces this repository records. The\n  estate splits three ways: a small set of open, unauthenticated campus and geospatial feeds; one\n  key-gated but freely self-serve research API; and an enterprise tier at the Texas A&M University\n  System that cannot\
  \ be reached at all without a sponsored account.\nauthentication:\n- surface: Texas A&M GeoServices Geocoding API\n  base_url: https://geoservices.tamu.edu/Api/Geocode/V5\n  x-operator: institution\n  scheme: api_key\n  mechanism: apiKey query parameter\n  public: true\n  self_service: true\n  evidence:\n  - url: https://geoservices.tamu.edu/Api/Geocode/V5/?version=5.0.0&streetAddress=1101%20Texas%20Ave&city=College%20Station&state=TX&zip=77840&format=json\n    status: 200\n    location: body.statusCode = 401, body.message = \"APIKeyMissing\", body.data.queryStatusCode = \"APIKeyMissing\"\n  - url: https://geoservices.tamu.edu/Signup/\n    status: 200\n    location: public self-service account signup issuing the API key\n  note: >-\n    The key travels in the query string, not a header. Texas A&M returns HTTP 200 for an\n    unauthenticated call and carries the real 401 inside the JSON body, which means naive status-code\n    monitoring will read this API as healthy while every request\
  \ is failing.\n- surface: Aggie Map Dining Locations API\n  base_url: https://api.aggiemap.tamu.edu\n  x-operator: institution\n  scheme: none\n  public: true\n  evidence:\n    url: https://api.aggiemap.tamu.edu/dining/locations/geojson\n    status: 200\n    location: 54-feature GeoJSON FeatureCollection returned to an anonymous request\n  note: >-\n    Open with no credential, no documented terms and no published rate limit. It is an application\n    backend, not an offered API, and should be treated as unguaranteed.\n- surface: Campus Micromobility Vehicle Positions\n  base_url: https://veoride.geoservices.tamu.edu\n  x-operator: institution\n  scheme: none\n  public: true\n  evidence:\n    url: https://veoride.geoservices.tamu.edu/api/vehicles/basic/geojson\n    status: 200\n    location: 3,300-feature GeoJSON FeatureCollection returned to an anonymous request\n- surface: Texas A&M IT ArcGIS REST Services\n  base_url: https://gis.it.tamu.edu/arcgis/rest/services\n  x-operator: institution\n\
  \  scheme: none\n  public: true\n  evidence:\n  - url: https://gis.it.tamu.edu/arcgis/rest/services?f=json\n    status: 200\n    location: 'currentVersion 11.5; folders FCOR, Hosted, Routing, System, Testing, TS, Utilities'\n  - url: https://gis.tamu.edu/arcgis/rest/services?f=json\n    status: 200\n    location: identical catalog served under a second Texas A&M hostname\n  note: >-\n    The services directory and its MapServer/FeatureServer children answer anonymously. The software\n    is Esri ArcGIS Server; the deployment, the hostnames and the published layers are Texas A&M's.\n- surface: OAKTrust Institutional Repository — OAI-PMH\n  base_url: https://oaktrust.library.tamu.edu/server/oai/request\n  x-operator: institution\n  scheme: none\n  public: true\n  evidence:\n  - url: https://oaktrust.library.tamu.edu/server/oai/request?verb=Identify\n    status: 200\n    location: 'OAI-PMH/Identify/repositoryName = \"OAKTrust\"; adminEmail helpdesk@library.tamu.edu'\n  - url: https://oaktrust.library.tamu.edu/oai/request?verb=Identify\n\
  \    status: 403\n    location: Cloudflare interstitial on the legacy DSpace 6 path\n  note: >-\n    The DSpace 7 path answers anonymously. The rest of the host — including the DSpace REST API at\n    /server/api and the Scholars@TAMU application — sits behind a Cloudflare bot challenge that\n    returns 403 to a browser User-Agent. That is a fact about our access, not about Texas A&M's\n    policy.\n- surface: Texas A&M University Identity Federation (Shibboleth IdP metadata)\n  base_url: https://idp.tamu.edu/idp/shibboleth\n  x-operator: institution\n  scheme: none\n  public: true\n  evidence:\n  - url: https://idp.tamu.edu/idp/shibboleth\n    status: 200\n    location: EntityDescriptor entityID urn:mace:tamu.edu:shibboleth:idp:tamu:administrative:cscn:idp.tamu.edu\n  - url: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Atamu.edu\n    status: 200\n    location: 'mdui:DisplayName \"Texas A&M University\"; SSO at idp.tamu.edu'\n  note: >-\n    Metadata is public by design; the\
  \ SSO endpoints it advertises are the authenticating surface for\n    everything else on campus.\n- surface: UIN Services API (Texas A&M University System)\n  base_url: not published\n  x-operator: institution\n  scheme: api_key\n  mechanism: x-api-key header\n  public: false\n  self_service: false\n  evidence:\n  - url: https://it.tamus.edu/uinmanager/api/\n    status: 200\n    location: >-\n      Access requires registering an application, subscribing to UIN Proxy Services v3 in the API\n      Catalog, and approval by the System Enterprise Applications (SEA) DevOps group\n  - url: https://api-doc.sea.system.tamus.edu/\n    status: 200\n    location: Axway-style GWT API Developer Portal shell; the catalog itself renders only after login\n  - url: https://api-doc.sea.system.tamus.edu/api/portal/v1.3/discovery/apis\n    status: 404\n    location: no unauthenticated discovery route responds on the portal\n  note: >-\n    The enterprise tier exists and is real, but no base URL, no specification\
  \ and no API inventory is\n    reachable without a sponsored System account. It is inventoried from Texas A&M's own\n    documentation and is never described here as callable.\n- surface: Canvas LMS\n  base_url: https://canvas.tamu.edu\n  x-operator: tenant\n  scheme: oauth2\n  public: false\n  evidence:\n    url: dns:canvas.tamu.edu\n    status: 200\n    location: CNAME to texasam-vanity.instructure.com\n  note: >-\n    Texas A&M's Canvas tenancy is real, but the REST API, its OAuth flows and its LTI conformance are\n    Instructure's contract, not Texas A&M's. Recorded as a relationship only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/texas-a-m-university/refs/heads/main/authentication/texas-a-m-university-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United States
- Texas
- Public Research University
- Land Grant
- Research
- Research Data
- Research Repository
- Identity Federation
- Geospatial
- Geocoding
- Open Data
- Library
- Course Catalog
- Campus Life
- Research Computing
---
