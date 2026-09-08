---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: centene-fhir-patient-access-openapi.json
  format: json
  label: Centene FHIR Patient Access API
  slug: centene-fhir-patient-access
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-fhir-patient-access-openapi.json
- filename: centene-fhir-provider-directory-openapi.json
  format: json
  label: Centene FHIR Provider Directory API
  slug: centene-fhir-provider-directory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-fhir-provider-directory-openapi.json
- filename: centene-provider-rtr-fhir-pdex-openapi.json
  format: json
  label: Centene Provider RTR - FHIR PDEX Directory API
  slug: centene-fhir-pdex-rtr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-provider-rtr-fhir-pdex-openapi.json
- filename: centene-provider-rtr-demographics-openapi.json
  format: json
  label: Centene Provider RTR Demographics API
  slug: centene-provider-rtr-demographics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-provider-rtr-demographics-openapi.json
- filename: centene-pces-openapi.yaml
  format: yaml
  label: Centene Provider Carrier Entity Search (PCES) API
  slug: centene-pces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-pces-openapi.yaml
- filename: centene-pces-extract-openapi.yaml
  format: yaml
  label: Centene Provider Carrier Entity Search (PCES) Extract API
  slug: centene-pces-extract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-pces-extract-openapi.yaml
- filename: centene-provider-search-suggest-openapi.yaml
  format: yaml
  label: Centene Provider Search Suggest API
  slug: centene-provider-search-suggest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-provider-search-suggest-openapi.yaml
- filename: centene-product-mapping-v2-openapi.yaml
  format: yaml
  label: Centene Product Mapping V2 API
  slug: centene-product-mapping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-product-mapping-v2-openapi.yaml
- filename: centene-edi-core-realtime-openapi.json
  format: json
  label: Centene LWC EDI CORE Real Time Service
  slug: centene-edi-core-realtime
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-edi-core-realtime-openapi.json
- filename: centene-ccm-communication-openapi.json
  format: json
  label: Centene CCM Communication API
  slug: centene-ccm-communication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-ccm-communication-openapi.json
- filename: centene-ccm-sms-userresponse-openapi.json
  format: json
  label: Centene CCM SMS User Response Webhook
  slug: centene-ccm-sms-userresponse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-ccm-sms-userresponse-openapi.json
- filename: centene-healow-health-openapi.yaml
  format: yaml
  label: Centene Healow Health API
  slug: centene-healow-health
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/openapi/centene-healow-health-openapi.yaml
auth_types:
- oauth2
- openIdConnect
- http
- apiKey
- none
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Centene Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Centene secures its APIs with oauth2, openIdConnect, http, apiKey, and none across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Centene
provider_slug: centene
scheme_count: 5
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://stage.entrykeyid.com/as/token.oauth2
  name: oauth2
  sources:
  - openapi/centene-provider-rtr-demographics-openapi.json
  - openapi/centene-provider-rtr-fhir-pdex-openapi.json
  type: oauth2
- name: Bearer
  scheme: bearer
  sources:
  - openapi/centene-fhir-patient-access-openapi.json
  type: http
- name: Basic
  note: Declared in three specs. For the Provider Directory this contradicts the catalogue entry and the live behaviour, both of which say the API is anonymous - treat the spec block as stale.
  scheme: basic
  sources:
  - openapi/centene-fhir-provider-directory-openapi.json
  - openapi/centene-product-mapping-v2-openapi.yaml
  - openapi/centene-provider-search-suggest-openapi.yaml
  type: http
- in: header
  name: api_key
  parameter: api_key
  sources:
  - openapi/centene-pces-openapi.yaml
  - openapi/centene-pces-extract-openapi.yaml
  type: apiKey
- in: header
  name: clientID
  parameter: APIKey
  sources:
  - openapi/centene-edi-core-realtime-openapi.json
  type: apiKey
slug: centene-authentication
source_filename: centene-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: https://partners.centene.com/apiDetail/2718669d-6e2e-42b5-8c90-0a82f13a30ba\ndocs:\n  - https://partners.centene.com/apiDetail/2718669d-6e2e-42b5-8c90-0a82f13a30ba\n  - https://partners.centene.com/apiDetail/8122bc9c-43d6-4a2a-b6be-2272df8b8566\n  - https://partners.centene.com/applicationDeveloper\n  - https://partners.centene.com/.well-known/openid-configuration\nprovider: Centene\nproviderId: centene\nnote: >-\n  Derived from the securitySchemes of all twelve first-party Centene OpenAPI documents, then\n  upgraded from two provider-published sources - the Getting Started guides attached to the FHIR\n  Patient Access and Provider Directory catalogue entries (fetched as Markdown from the partner\n  portal's own document service), and the OpenID Provider Metadata document served at\n  partners.centene.com/.well-known/openid-configuration. Centene runs a single Ping Identity\n  authorization server, branded EntryKey ID, across\
  \ all published APIs; the OpenAPI documents\n  disagree with the portal on scheme in several places because the specs were authored per-team\n  and the gateway enforces OAuth uniformly in front of them.\nsummary:\n  primary_model: oauth2\n  authorization_server: https://sso.entrykeyid.com\n  sandbox_authorization_server: https://sandbox.entrykeyid.com\n  identity_brand: EntryKey ID (Ping Identity PingFederate)\n  types:\n    - oauth2\n    - openIdConnect\n    - http\n    - apiKey\n    - none\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorizationCode\n    - clientCredentials\n  pkce: supported (S256)\n  mtls: not published\n  token_lifetime_seconds: 3600\n  refresh_tokens: supported\n  dynamic_client_registration: >-\n    registration_endpoint is advertised (https://sso.entrykeyid.com/as/clients.oauth2) but Centene\n    routes real onboarding through the Third-Party Application Developer form, not anonymous DCR.\nonboarding:\n  model: application-registration\n  form: https://partners.centene.com/applicationDeveloper-form\n\
  \  overview: https://partners.centene.com/applicationDeveloper\n  contact: IOP_External_Onboarding@Centene.com\n  note: >-\n    A developer registers an application through the partner portal, is issued a clientId and\n    clientSecret, and supplies a redirect_uri. Client credentials are exchanged with HTTP Basic\n    (base64(clientId:clientSecret)) at the token endpoint. No self-service key issuance.\nflows:\n  - id: smart-standalone-member-authorization\n    name: SMART on FHIR standalone launch (member-authorized)\n    used_by:\n      - FHIR - Patient Access\n    grant_type: authorization_code\n    implementation_guide: HL7 SMART App Launch Framework IG 2.0.0\n    authorize_url: https://sandbox.entrykeyid.com/as/authorization.oauth2\n    token_url: https://sandbox.entrykeyid.com/as/token.oauth2\n    production_authorize_url: https://sso.entrykeyid.com/as/authorization.oauth2\n    production_token_url: https://sso.entrykeyid.com/as/token.oauth2\n    request_scopes: ['patient/*.read',\
  \ openid]\n    granted_scope_example: Patient/*.read launch/patient offline_access\n    token_request_auth: HTTP Basic base64(clientId:clientSecret)\n    token_request_content_type: application/json\n    authorization_code_reuse: >-\n      Single use. Centene's guide states plainly - \"Please note the Authorization Code is only\n      valid for a single use.\"\n    access_token_ttl_seconds: 3600\n    refresh: >-\n      A refresh_token is returned and can be exchanged at the same token endpoint with\n      grant_type=refresh_token, so an app can keep syncing member data without re-running the\n      consent flow.\n    patient_context: >-\n      The token response carries a top-level `patient` claim holding the FHIR Patient logical id\n      the token is scoped to.\n    ehr_launch: not implemented\n  - id: client-credentials-service-account\n    name: Client Credentials (Service Account)\n    used_by:\n      - Provider RTR - FHIR PDEX Directory API (External)\n      - Provider RTR - Demographics\
  \ API\n      - Provider Carrier Entity Search (PCES) API\n      - Provider Carrier Entity Search (PCES) Extract API\n      - Provider Search Suggest API\n      - Product Mapping V2\n      - LWC EDI CORE REAL TIME SERVICE\n      - CCM Communication\n      - Healow API\n    grant_type: client_credentials\n    token_url: https://stage.entrykeyid.com/as/token.oauth2\n    scopes: [resource.read, openid, profile]\n    audience_required: true\n    audience_note: >-\n      Every catalogue entry carries an `audience` value (patientaccess, prtrdemographic, ewsext,\n      edicorertservice, CCMAPIUSER, edas, xkafdev). The gateway validates it, so a token minted\n      for one Centene API will not open another.\n  - id: public-no-auth\n    name: Anonymous\n    used_by:\n      - FHIR - Provider Directory\n    grant_type: none\n    note: >-\n      The catalogue entry records authentication \"None\" and an empty scope list, and this was\n      verified live - GET on the production Practitioner endpoint\
  \ returned HTTP 200 with a FHIR\n      searchset Bundle with no credential of any kind. CMS requires payer provider-directory data\n      to be publicly accessible without member authorization.\nschemes:\n  - name: oauth2\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://stage.entrykeyid.com/as/token.oauth2\n        scopes: 1\n    sources:\n      - openapi/centene-provider-rtr-demographics-openapi.json\n      - openapi/centene-provider-rtr-fhir-pdex-openapi.json\n  - name: Bearer\n    type: http\n    scheme: bearer\n    sources:\n      - openapi/centene-fhir-patient-access-openapi.json\n  - name: Basic\n    type: http\n    scheme: basic\n    note: >-\n      Declared in three specs. For the Provider Directory this contradicts the catalogue entry and\n      the live behaviour, both of which say the API is anonymous - treat the spec block as stale.\n    sources:\n      - openapi/centene-fhir-provider-directory-openapi.json\n      - openapi/centene-product-mapping-v2-openapi.yaml\n\
  \      - openapi/centene-provider-search-suggest-openapi.yaml\n  - name: api_key\n    type: apiKey\n    in: header\n    parameter: api_key\n    sources:\n      - openapi/centene-pces-openapi.yaml\n      - openapi/centene-pces-extract-openapi.yaml\n  - name: clientID\n    type: apiKey\n    in: header\n    parameter: APIKey\n    sources:\n      - openapi/centene-edi-core-realtime-openapi.json\ngaps:\n  - >-\n    The OpenAPI documents do not declare the OAuth 2.0 authorization server the gateway actually\n    enforces; only two of twelve carry an oauth2 securityScheme, and those point at a staging\n    token endpoint (stage.entrykeyid.com) rather than production.\n  - >-\n    No securityScheme in any published spec references the SMART on FHIR scopes, so an agent\n    reading only the Patient Access OpenAPI would request no scopes and be rejected.\n  - No mutual TLS, DPoP, signed-request or token-binding requirement is published.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centene/refs/heads/main/authentication/centene-authentication.yml
summary_line: oauth2/openIdConnect/http/apiKey/none · 5 schemes
tags:
- Healthcare
- Insurance
- Managed Care
- FHIR
- HL7
- CMS Interoperability
- Patient Access
- Provider Directory
- Payer
- Medicaid
- Medicare
- Interoperability
- SMART on FHIR
- PDEX
- CARIN Blue Button
- US Core
- Formulary
- X12
- EDI
- Fortune 500
---
