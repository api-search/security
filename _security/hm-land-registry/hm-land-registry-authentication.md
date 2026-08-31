---
api_key_in:
- header
api_specs:
- filename: hm-land-registry-application-information-api-api-openapi.yml
  format: yaml
  label: HM Land Registry Application information API
  slug: hm-land-registry-application-information-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-application-information-api-api-openapi.yml
- filename: hm-land-registry-attach-a-document-api-openapi.yml
  format: yaml
  label: HM Land Registry Attach a document API
  slug: hm-land-registry-attach-a-document-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-attach-a-document-api-openapi.yml
- filename: hm-land-registry-attach-a-message-api-openapi.yml
  format: yaml
  label: HM Land Registry Attach a message API
  slug: hm-land-registry-attach-a-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-attach-a-message-api-openapi.yml
- filename: hm-land-registry-datasets-api-openapi.yml
  format: yaml
  label: HM Land Registry Datasets API
  slug: hm-land-registry-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-datasets-api-openapi.yml
- filename: hm-land-registry-download-a-document-api-api-openapi.yml
  format: yaml
  label: HM Land Registry Download a document API
  slug: hm-land-registry-download-a-document-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-download-a-document-api-api-openapi.yml
- filename: hm-land-registry-draft-titles-api-openapi.yml
  format: yaml
  label: HM Land Registry Draft Titles API
  slug: hm-land-registry-draft-titles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-draft-titles-api-openapi.yml
- filename: hm-land-registry-ecd-api-openapi.yml
  format: yaml
  label: HM Land Registry ECD API
  slug: hm-land-registry-ecd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-ecd-api-openapi.yml
- filename: hm-land-registry-notifications-api-api-openapi.yml
  format: yaml
  label: HM Land Registry Notifications API
  slug: hm-land-registry-notifications-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-notifications-api-api-openapi.yml
- filename: hm-land-registry-official-copies-api-openapi.yml
  format: yaml
  label: HM Land Registry Official Copies API
  slug: hm-land-registry-official-copies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-official-copies-api-openapi.yml
- filename: hm-land-registry-official-search-of-whole-with-data-api-openapi.yml
  format: yaml
  label: HM Land Registry Official Search of Whole with Data API
  slug: hm-land-registry-official-search-of-whole-with-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-official-search-of-whole-with-data-api-openapi.yml
- filename: hm-land-registry-registered-proprietor-names-api-openapi.yml
  format: yaml
  label: HM Land Registry Registered Proprietor Names API
  slug: hm-land-registry-registered-proprietor-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-registered-proprietor-names-api-openapi.yml
- filename: hm-land-registry-send-a-document-api-api-openapi.yml
  format: yaml
  label: HM Land Registry Send a document API
  slug: hm-land-registry-send-a-document-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-send-a-document-api-api-openapi.yml
- filename: hm-land-registry-submit-an-application-api-api-openapi.yml
  format: yaml
  label: HM Land Registry Submit an application API
  slug: hm-land-registry-submit-an-application-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-submit-an-application-api-api-openapi.yml
- filename: hm-land-registry-title-api-openapi.yml
  format: yaml
  label: HM Land Registry Title API
  slug: hm-land-registry-title-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-title-api-openapi.yml
- filename: hm-land-registry-titles-api-openapi.yml
  format: yaml
  label: HM Land Registry Titles API
  slug: hm-land-registry-titles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/openapi/hm-land-registry-titles-api-openapi.yml
auth_types:
- http
- apiKey
- none
description: ''
kind: authentication
layout: security
method: searched
name: Hm Land Registry Authentication
name_suffix: Authentication
oauth_flows: []
overview: HM Land Registry secures its APIs with http, apiKey, and none across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HM Land Registry
provider_slug: hm-land-registry
scheme_count: 5
schemes:
- docs: https://landregistry.github.io/bgtechdoc/rest/get_started/developer_guide/index.html
  name: basicAuth
  note: Username and password for an active Business Gateway user account, sent as HTTP Basic. Only meaningful inside the mutual-TLS session; without the client certificate the connection never reaches the point of returning 401.
  scheme: basic
  sources:
  - openapi/hm-land-registry-estimate-completion-date-openapi.yml
  - openapi/hm-land-registry-official-copy-document-availability-v1-openapi.json
  - openapi/hm-land-registry-official-copy-document-availability-v2-openapi.json
  - openapi/hm-land-registry-registered-proprietor-names-openapi.json
  - openapi/hm-land-registry-submit-application-to-change-the-register-v0.3-openapi.json
  - openapi/hm-land-registry-submit-application-to-change-the-register-v1.0-openapi.json
  type: http
- bearerFormat: UUID
  name: bearerAuth
  note: Land Register API only, an internal HMLR API. A token is minted per consuming service by the Digital Register project team; the consumer must file a Fraud Impact Assessment and must not expose the data externally. Not obtainable as a developer.
  scheme: bearer
  sources:
  - openapi/hm-land-registry-land-register-api-openapi.yml
  type: http
- docs: https://use-land-property-data.service.gov.uk/api-documentation
  in: header
  issuance: Issued automatically on self-serve account creation at https://use-land-property-data.service.gov.uk/registration
  name: apiKey
  note: 'Sent as the Authorization header on every request; Accept: application/json is advised. Verified 2026-07-26: calling without it returns HTTP 403 "Access denied: You need to provide your API Key to perform this operation".'
  parameter_name: Authorization
  sources:
  - openapi/hm-land-registry-use-land-property-data-openapi.yml
  type: apiKey
- docs: https://landregistry.github.io/bgtechdoc/rest/get_started/developer_guide/index.html
  name: mutualTLS
  note: 'A valid client digital certificate issued by Business Gateway must be installed in the client key store, and HMLR-issued certificates trusted as root. Probed 2026-07-26: businessgateway.landregistry.gov.uk and bgtest.landregistry.gov.uk refuse the TLS handshake without it. This control is invisible to any client generated from the published contracts.'
  sources:
  - documented, not declared in any OpenAPI
  type: mutualTLS
- name: none
  note: The SPARQL 1.1 endpoint and the Price Paid / UK House Price Index Linked Data APIs are anonymous. Verified HTTP 200 without credentials on 2026-07-26.
  sources:
  - apis.yml open-data APIs
  type: none
slug: hm-land-registry-authentication
source_filename: hm-land-registry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/hm-land-registry-estimate-completion-date-openapi.yml, openapi/hm-land-registry-land-register-api-openapi.yml,\n  openapi/hm-land-registry-official-copy-document-availability-v1-openapi.json, openapi/hm-land-registry-official-copy-document-availability-v2-openapi.json,\n  openapi/hm-land-registry-registered-proprietor-names-openapi.json, openapi/hm-land-registry-submit-application-to-change-the-register-v0.3-openapi.json,\n  openapi/hm-land-registry-submit-application-to-change-the-register-v1.0-openapi.json\nsummary:\n  types:\n  - http\n  - apiKey\n  - none\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: 'Three estates, three models, and no OAuth anywhere. Business Gateway is HTTP Basic carried inside\n    a mutual-TLS session established with an HMLR-issued client certificate — the certificate is the real\n    gate and it is not modelled in any OpenAPI securityScheme. Use land and property data is a simple\n\
  \    API key in the Authorization header, self-serve on account creation, with a second gate behind it:\n    a signed per-dataset licence. The open linked-data platform requires no credential at all. The internal\n    Land Register API is the only bearer-token surface and is not a developer product.'\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/hm-land-registry-estimate-completion-date-openapi.yml\n  - openapi/hm-land-registry-official-copy-document-availability-v1-openapi.json\n  - openapi/hm-land-registry-official-copy-document-availability-v2-openapi.json\n  - openapi/hm-land-registry-registered-proprietor-names-openapi.json\n  - openapi/hm-land-registry-submit-application-to-change-the-register-v0.3-openapi.json\n  - openapi/hm-land-registry-submit-application-to-change-the-register-v1.0-openapi.json\n  docs: https://landregistry.github.io/bgtechdoc/rest/get_started/developer_guide/index.html\n  note: Username and password for an active Business\
  \ Gateway user account, sent as HTTP Basic. Only meaningful\n    inside the mutual-TLS session; without the client certificate the connection never reaches the point\n    of returning 401.\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: UUID\n  sources:\n  - openapi/hm-land-registry-land-register-api-openapi.yml\n  note: Land Register API only, an internal HMLR API. A token is minted per consuming service by the Digital\n    Register project team; the consumer must file a Fraud Impact Assessment and must not expose the data\n    externally. Not obtainable as a developer.\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  sources:\n  - openapi/hm-land-registry-use-land-property-data-openapi.yml\n  docs: https://use-land-property-data.service.gov.uk/api-documentation\n  issuance: Issued automatically on self-serve account creation at https://use-land-property-data.service.gov.uk/registration\n  note: 'Sent as the Authorization header on\
  \ every request; Accept: application/json is advised. Verified\n    2026-07-26: calling without it returns HTTP 403 \"Access denied: You need to provide your API Key to\n    perform this operation\".'\n- name: mutualTLS\n  type: mutualTLS\n  sources:\n  - documented, not declared in any OpenAPI\n  docs: https://landregistry.github.io/bgtechdoc/rest/get_started/developer_guide/index.html\n  note: 'A valid client digital certificate issued by Business Gateway must be installed in the client\n    key store, and HMLR-issued certificates trusted as root. Probed 2026-07-26: businessgateway.landregistry.gov.uk\n    and bgtest.landregistry.gov.uk refuse the TLS handshake without it. This control is invisible to any\n    client generated from the published contracts.'\n- name: none\n  type: none\n  sources:\n  - apis.yml open-data APIs\n  note: The SPARQL 1.1 endpoint and the Price Paid / UK House Price Index Linked Data APIs are anonymous.\n    Verified HTTP 200 without credentials on 2026-07-26.\n\
  docs:\n- https://landregistry.github.io/bgtechdoc/rest/get_started/developer_guide/index.html\n- https://landregistry.github.io/bg-dev-pack-redesign/how-to-access-business-gateway\n- https://use-land-property-data.service.gov.uk/api-documentation\nonboarding:\n  business_gateway:\n    self_serve: false\n    steps:\n    - Sign the development licence (request from channelpartners@landregistry.gov.uk).\n    - HMLR sends a test SSL certificate to the named technical contact.\n    - Build with support from the integration support team.\n    - Hold a business e-services account, then contact HMLR for live access.\n    docs: https://landregistry.github.io/bg-dev-pack-redesign/how-to-access-business-gateway\n  use_land_and_property_data:\n    self_serve: true\n    steps:\n    - Create an account; an API key is issued automatically.\n    - Sign the licence for each dataset you want.\n    - Pay where the dataset is chargeable.\n    docs: https://use-land-property-data.service.gov.uk/registration\n\
  \  open_data:\n    self_serve: true\n    steps:\n    - None. Call the endpoint.\noauth:\n  supported: false\n  detail: No oauth2 or openIdConnect scheme anywhere in the estate; no /.well-known/oauth-authorization-server\n    or /.well-known/openid-configuration on any host (probed 2026-07-26). scopes/ is therefore intentionally\n    absent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hm-land-registry/refs/heads/main/authentication/hm-land-registry-authentication.yml
summary_line: http/apiKey/none · 5 schemes
tags:
- Real-Estate
- United Kingdom
- Land Registry
- Open Data
- Title
- Conveyancing
- Property Records
- Price Paid Data
- Linked Data
- Geospatial
- Government
- PropTech
---
