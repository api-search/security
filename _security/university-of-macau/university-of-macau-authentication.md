---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: university-of-macau-access-control-records-api-openapi.yml
  format: yaml
  label: University of Macau Access Control Records API
  slug: university-of-macau-access-control-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-access-control-records-api-openapi.yml
- filename: university-of-macau-car-park-availability-api-openapi.yml
  format: yaml
  label: University of Macau Car Park Availability API
  slug: university-of-macau-car-park-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-car-park-availability-api-openapi.yml
- filename: university-of-macau-computer-room-pc-status-api-openapi.yml
  format: yaml
  label: University of Macau Computer Room PC Status API
  slug: university-of-macau-computer-room-pc-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-computer-room-pc-status-api-openapi.yml
- filename: university-of-macau-computer-room-reservations-api-openapi.yml
  format: yaml
  label: University of Macau Computer Room Reservations API
  slug: university-of-macau-computer-room-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-computer-room-reservations-api-openapi.yml
- filename: university-of-macau-course-catalog-api-openapi.yml
  format: yaml
  label: University of Macau Course Catalog API
  slug: university-of-macau-course-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-course-catalog-api-openapi.yml
- filename: university-of-macau-courses-api-openapi.yml
  format: yaml
  label: University of Macau Courses API
  slug: university-of-macau-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-courses-api-openapi.yml
- filename: university-of-macau-events-api-openapi.yml
  format: yaml
  label: University of Macau Events API
  slug: university-of-macau-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-events-api-openapi.yml
- filename: university-of-macau-news-api-openapi.yml
  format: yaml
  label: University of Macau News API
  slug: university-of-macau-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-news-api-openapi.yml
- filename: university-of-macau-organizational-units-api-openapi.yml
  format: yaml
  label: University of Macau Organizational Units API
  slug: university-of-macau-organizational-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-organizational-units-api-openapi.yml
- filename: university-of-macau-public-holidays-api-openapi.yml
  format: yaml
  label: University of Macau Public Holidays API
  slug: university-of-macau-public-holidays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-public-holidays-api-openapi.yml
- filename: university-of-macau-rc-hostel-bed-spaces-api-openapi.yml
  format: yaml
  label: University of Macau RC Hostel Bed Spaces API
  slug: university-of-macau-rc-hostel-bed-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-rc-hostel-bed-spaces-api-openapi.yml
- filename: university-of-macau-shuttle-bus-arrival-time-api-openapi.yml
  format: yaml
  label: University of Macau Shuttle Bus Arrival Time API
  slug: university-of-macau-shuttle-bus-arrival-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-shuttle-bus-arrival-time-api-openapi.yml
- filename: university-of-macau-sports-facilities-api-openapi.yml
  format: yaml
  label: University of Macau Sports Facilities API
  slug: university-of-macau-sports-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-sports-facilities-api-openapi.yml
- filename: university-of-macau-sports-facilities-booking-api-openapi.yml
  format: yaml
  label: University of Macau Sports Facilities Booking API
  slug: university-of-macau-sports-facilities-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-sports-facilities-booking-api-openapi.yml
- filename: university-of-macau-student-job-vacancies-api-openapi.yml
  format: yaml
  label: University of Macau Student Job Vacancies API
  slug: university-of-macau-student-job-vacancies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-student-job-vacancies-api-openapi.yml
- filename: university-of-macau-wifi-access-log-api-openapi.yml
  format: yaml
  label: University of Macau Wifi Access Log API
  slug: university-of-macau-wifi-access-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/openapi/university-of-macau-wifi-access-log-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: University Of Macau Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Macau secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Macau
provider_slug: university-of-macau
scheme_count: 2
schemes:
- evidence: subscriptionKeyParameterNames.header = "Authorization" on all 16 APIs in the developer-portal metadata; live 401 challenge names the same header.
  format: raw subscription key (no "Bearer " prefix)
  in: header
  issuance: Register the "OPEN DATA API PLATFORM" service on the ICTO Account Information page, sign in to data.um.edu.mo with UMPASS, subscribe to the "UM Members" product, then reveal the Primary or Secondary key on the Subscriptions page. Two keys are issued per subscription, which is the Azure API Management rotation model (rotate one while the other stays live).
  name: apiKeyHeader
  parameter: Authorization
  purpose: Call any of the 16 data-set APIs on https://api.data.um.edu.mo.
  type: apiKey
- evidence: subscriptionKeyParameterNames.query = "subscription-key" on all 16 APIs.
  in: query
  name: apiKeyQuery
  parameter: subscription-key
  purpose: Same key, supplied on the query string instead of the header.
  type: apiKey
slug: university-of-macau-authentication
source_filename: university-of-macau-authentication.yml
source_heading: Authentication Profile
source_url: https://data.um.edu.mo/quickstart
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: https://api.data.um.edu.mo/service/media/events/all\ndocs: https://data.um.edu.mo/quickstart\nsources:\n- https://data.um.edu.mo/quickstart\n- https://data.um.edu.mo/developer/apis?api-version=2022-04-01-preview\n- https://api.data.um.edu.mo/service/media/events/all\n- https://login.microsoftonline.com/getuserrealm.srf?login=user@um.edu.mo&json=1\nx-operator: institution\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  note: >-\n    Two credentials, two different populations. The Data and Open Data API itself is protected by\n    an Azure API Management subscription key with no OAuth flow and no scope model at all: the\n    gateway answers an unauthenticated call with 401 and\n    `WWW-Authenticate: AzureApiManagementKey realm=\"https://api.data.um.edu.mo/service/media/events\",\n    name=\"Authorization\", type=\"header\"`. Obtaining that key is what is actually gated — it requires\n\
  \    a UMPASS account, which requires University of Macau affiliation. So the API is not public in\n    the sense a developer means it: anyone can read the surface, nobody outside UM can call it.\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: raw subscription key (no \"Bearer \" prefix)\n  purpose: Call any of the 16 data-set APIs on https://api.data.um.edu.mo.\n  issuance: >-\n    Register the \"OPEN DATA API PLATFORM\" service on the ICTO Account Information page, sign in to\n    data.um.edu.mo with UMPASS, subscribe to the \"UM Members\" product, then reveal the Primary or\n    Secondary key on the Subscriptions page. Two keys are issued per subscription, which is the\n    Azure API Management rotation model (rotate one while the other stays live).\n  evidence: >-\n    subscriptionKeyParameterNames.header = \"Authorization\" on all 16 APIs in the developer-portal\n    metadata; live 401 challenge names the same header.\n- name: apiKeyQuery\n\
  \  type: apiKey\n  in: query\n  parameter: subscription-key\n  purpose: Same key, supplied on the query string instead of the header.\n  evidence: subscriptionKeyParameterNames.query = \"subscription-key\" on all 16 APIs.\nidentity:\n  gate: UMPASS\n  gate_operator: institution\n  note: >-\n    UMPASS is the University of Macau's own single sign-on. The realm lookup for um.edu.mo returns\n    NameSpaceType \"Federated\" with AuthURL https://websso.um.edu.mo/adfs/ls/ and FederationBrandName\n    \"University of Macau\" — that is UM's own AD FS identity provider, federated into a Microsoft\n    Entra ID tenant (76eeec46-fe40-4e1b-ab42-1d6d9f91b8a9). The IdP is institution-operated; only\n    the federation broker is Microsoft's.\n  metadata:\n  - kind: saml2-metadata\n    url: https://websso.um.edu.mo/FederationMetadata/2007-06/FederationMetadata.xml\n    status: 200\n    content_type: application/samlmetadata+xml\n    entity_id: http://websso.um.edu.mo/adfs/services/trust\n  - kind: openid-configuration\n\
  \    url: https://websso.um.edu.mo/adfs/.well-known/openid-configuration\n    status: 200\n    issuer: https://websso.umac.mo/adfs\n  - kind: entra-openid-configuration\n    url: https://login.microsoftonline.com/um.edu.mo/v2.0/.well-known/openid-configuration\n    status: 200\n    issuer: https://login.microsoftonline.com/76eeec46-fe40-4e1b-ab42-1d6d9f91b8a9/v2.0\nscopes:\n  model: none\n  detail: >-\n    No OAuth2 or OpenID Connect authentication settings are configured on any of the 16 APIs\n    (authenticationSettings.oAuth2AuthenticationSettings and .openidAuthenticationSettings are both\n    empty arrays on every one). Authorization is coarse: a subscription to a product grants all\n    APIs in that product. There are no per-dataset or per-operation scopes to record.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-macau/refs/heads/main/authentication/university-of-macau-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- University
- Higher Education
- Education
- Public Research University
- Macau
- China
- Open Data
- Course Catalog
- Campus Life
- Identity Federation
- Research Repository
- Library
---
