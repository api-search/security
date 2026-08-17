---
api_key_in: []
api_specs:
- filename: jefferson-health-allergy-intolerance-api-openapi.yml
  format: yaml
  label: Jefferson Health Allergy Intolerance API
  slug: jefferson-health-allergy-intolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-allergy-intolerance-api-openapi.yml
- filename: jefferson-health-bulk-data-api-openapi.yml
  format: yaml
  label: Jefferson Health Bulk Data API
  slug: jefferson-health-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-bulk-data-api-openapi.yml
- filename: jefferson-health-condition-api-openapi.yml
  format: yaml
  label: Jefferson Health Condition API
  slug: jefferson-health-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-condition-api-openapi.yml
- filename: jefferson-health-document-reference-api-openapi.yml
  format: yaml
  label: Jefferson Health Document Reference API
  slug: jefferson-health-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-document-reference-api-openapi.yml
- filename: jefferson-health-encounter-api-openapi.yml
  format: yaml
  label: Jefferson Health Encounter API
  slug: jefferson-health-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-encounter-api-openapi.yml
- filename: jefferson-health-endpoint-api-openapi.yml
  format: yaml
  label: Jefferson Health Endpoint API
  slug: jefferson-health-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-endpoint-api-openapi.yml
- filename: jefferson-health-healthcare-service-api-openapi.yml
  format: yaml
  label: Jefferson Health Healthcare Service API
  slug: jefferson-health-healthcare-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-healthcare-service-api-openapi.yml
- filename: jefferson-health-insurance-plan-api-openapi.yml
  format: yaml
  label: Jefferson Health Insurance Plan API
  slug: jefferson-health-insurance-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-insurance-plan-api-openapi.yml
- filename: jefferson-health-location-api-openapi.yml
  format: yaml
  label: Jefferson Health Location API
  slug: jefferson-health-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-location-api-openapi.yml
- filename: jefferson-health-medication-request-api-openapi.yml
  format: yaml
  label: Jefferson Health Medication Request API
  slug: jefferson-health-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-medication-request-api-openapi.yml
- filename: jefferson-health-metadata-api-openapi.yml
  format: yaml
  label: Jefferson Health Metadata API
  slug: jefferson-health-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-metadata-api-openapi.yml
- filename: jefferson-health-observation-api-openapi.yml
  format: yaml
  label: Jefferson Health Observation API
  slug: jefferson-health-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-observation-api-openapi.yml
- filename: jefferson-health-organization-api-openapi.yml
  format: yaml
  label: Jefferson Health Organization API
  slug: jefferson-health-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-organization-api-openapi.yml
- filename: jefferson-health-patient-api-openapi.yml
  format: yaml
  label: Jefferson Health Patient API
  slug: jefferson-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-patient-api-openapi.yml
- filename: jefferson-health-practitioner-api-openapi.yml
  format: yaml
  label: Jefferson Health Practitioner API
  slug: jefferson-health-practitioner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-practitioner-api-openapi.yml
- filename: jefferson-health-practitioner-role-api-openapi.yml
  format: yaml
  label: Jefferson Health Practitioner Role API
  slug: jefferson-health-practitioner-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/openapi/jefferson-health-practitioner-role-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- none
description: Jefferson Health runs two independent authorization surfaces that share a brand and nothing else. The Thomas Jefferson University Hospital clinical FHIR endpoint requires a patient- or user-authorized SMART on FHIR token for every resource. The Jefferson Health Plans Da Vinci Plan-Net provider directory is served ANONYMOUSLY, as the implementation guide requires; its SMART authorization server exists for the separate Patient Access API and lives on a third host, appgallery.healthpartnersplans.com.
kind: authentication
layout: security
method: probed
name: Jefferson Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- jwtBearer
- tokenExchange
overview: Jefferson Health secures its APIs with oauth2, openIdConnect, and none across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, jwtBearer, and tokenExchange flow(s).
provider_name: Jefferson Health
provider_slug: jefferson-health
scheme_count: 3
schemes:
- applies_to: https://fhir.jefferson.edu/FHIRProxy/api/FHIR/R4
  backend_services: true
  backend_services_evidence: private_key_jwt + jwt-bearer grant + a published jwks_uri is the SMART Backend Services (system-level) shape, which is what the Bulk Data export requires.
  code_challenge_methods_supported:
  - S256
  description: SMART App Launch over OAuth 2.0 with mandatory PKCE. Covers both patient-facing standalone launches and provider-facing EHR launches.
  flows:
  - authorizationUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/authorize
    flow: authorizationCode
    scopes: 13
    tokenUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  - client_credentials
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  - urn:ietf:params:oauth:grant-type:token-exchange
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://fhir.jefferson.edu/FHIRProxy/oauth2
  jwks_uri: https://fhir.jefferson.edu/FHIRProxy/api/epic/2019/Security/Open/PublicKeys/530027/OIDC
  name: smartOnFhir
  pkce_required: true
  registration: https://fhir.epic.com/Developer/Apps
  registration_note: Client registration is handled by Epic on FHIR, not by Jefferson Health directly; Jefferson approves the app for production against its own endpoint.
  required: true
  response_modes_supported:
  - query
  response_types_supported:
  - code
  server: tjuh-fhir-r4
  smart_capabilities:
  - launch-ehr
  - launch-standalone
  - client-public
  - client-confidential-symmetric
  - client-confidential-asymmetric
  - context-banner
  - context-style
  - context-ehr-patient
  - context-ehr-encounter
  - context-standalone-patient
  - permission-offline
  - permission-patient
  - permission-user
  - permission-v1
  - permission-v2
  - sso-openid-connect
  - authorize-post
  sources:
  - well-known/jefferson-health-tjuh-smart-configuration.json
  - well-known/jefferson-health-tjuh-openid-configuration.json
  - conformance/jefferson-health-tjuh-fhir-r4-capabilitystatement.json
  - openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml
  subject_types_supported:
  - public
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: oauth2
- applies_to: https://smilercdr.healthpartnersplans.com/
  code_challenge_methods_supported:
  - plain
  - S256
  description: Jefferson Health Plans SMART on FHIR authorization server for the CARIN Blue Button Patient Access API. Developer registration runs through the JHP App Gallery developer portal.
  flows:
  - authorizationUrl: https://appgallery.healthpartnersplans.com/smartauth-fhir/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://appgallery.healthpartnersplans.com/smartauth-fhir/oauth/token
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://appgallery.healthpartnersplans.com/smartauth-fhir/oauth/token/introspect
  issuer: https://appgallery.healthpartnersplans.com/smartauth-fhir
  jwks_uri: https://appgallery.healthpartnersplans.com/smartauth-fhir/jwk
  name: jhpSmartAuth
  pkce_note: '''plain'' is advertised alongside S256. Clients should insist on S256; the server permitting ''plain'' is a weaker posture than the hospital endpoint, which offers S256 only.'
  pkce_required: false
  registration: https://appgallery.healthpartnersplans.com/app-gallery/portal/
  required: true
  response_types_supported:
  - code
  - code id_token
  - token
  - token id_token
  revocation_endpoint: https://appgallery.healthpartnersplans.com/smartauth-fhir/oauth/token/revoke
  server: jhp-patient-access
  session_management_endpoint: https://appgallery.healthpartnersplans.com/smartauth-fhir/session/management
  sources:
  - well-known/jefferson-health-jhp-openid-configuration.json
  - conformance/jefferson-health-jhp-provider-directory-capabilitystatement.json
  subject_types_supported:
  - public
  type: oauth2
  userinfo_endpoint: https://appgallery.healthpartnersplans.com/smartauth-fhir/userinfo
- applies_to: https://providerfhirapi.healthpartnersplans.com
  description: 'The Da Vinci Plan-Net provider directory requires no credentials. Verified live: GET /InsurancePlan?_count=1 and GET /Practitioner?_count=2 both returned HTTP 200 searchset Bundles with no Authorization header.'
  name: anonymous
  note: The CapabilityStatement still advertises SMART oauth-uris pointing at the appgallery authorization server, which is a decoy for this host — do not build an auth flow for the directory.
  required: false
  server: jhp-provider-directory
  type: none
slug: jefferson-health-authentication
source_filename: jefferson-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: >-\n  Live discovery documents fetched 2026-08-15 —\n  https://fhir.jefferson.edu/FHIRProxy/api/FHIR/R4/.well-known/smart-configuration,\n  https://fhir.jefferson.edu/FHIRProxy/api/FHIR/R4/.well-known/openid-configuration,\n  https://appgallery.healthpartnersplans.com/smartauth-fhir/.well-known/openid-configuration,\n  and the security blocks of both live CapabilityStatements. Supersedes the\n  2026-07-11 pass, which was derived from\n  openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml alone.\ndocs:\n  - https://www.jeffersonhealthplans.com/home/about-us/interoperability/authentication-and-data-endpoints/\n  - https://fhir.epic.com/Documentation\ndescription: >-\n  Jefferson Health runs two independent authorization surfaces that share a\n  brand and nothing else. The Thomas Jefferson University Hospital clinical FHIR\n  endpoint requires a patient- or user-authorized SMART on FHIR token for every\n  resource. The\
  \ Jefferson Health Plans Da Vinci Plan-Net provider directory is\n  served ANONYMOUSLY, as the implementation guide requires; its SMART\n  authorization server exists for the separate Patient Access API and lives on a\n  third host, appgallery.healthpartnersplans.com.\n\nsummary:\n  types: [oauth2, openIdConnect, none]\n  oauth2_flows: [authorizationCode, clientCredentials, jwtBearer, tokenExchange]\n  api_key_in: []\n  anonymous_surfaces: 1\n  authorization_servers: 2\n\nschemes:\n  - name: smartOnFhir\n    type: oauth2\n    server: tjuh-fhir-r4\n    applies_to: https://fhir.jefferson.edu/FHIRProxy/api/FHIR/R4\n    required: true\n    description: >-\n      SMART App Launch over OAuth 2.0 with mandatory PKCE. Covers both\n      patient-facing standalone launches and provider-facing EHR launches.\n    issuer: https://fhir.jefferson.edu/FHIRProxy/oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/authorize\n       \
  \ tokenUrl: https://fhir.jefferson.edu/FHIRProxy/oauth2/token\n        scopes: 13\n    grant_types_supported:\n      - authorization_code\n      - refresh_token\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n      - urn:ietf:params:oauth:grant-type:token-exchange\n    token_endpoint_auth_methods_supported:\n      - client_secret_post\n      - client_secret_basic\n      - private_key_jwt\n    code_challenge_methods_supported: [S256]\n    pkce_required: true\n    response_types_supported: [code]\n    response_modes_supported: [query]\n    jwks_uri: https://fhir.jefferson.edu/FHIRProxy/api/epic/2019/Security/Open/PublicKeys/530027/OIDC\n    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported: [public]\n    smart_capabilities:\n      - launch-ehr\n      - launch-standalone\n      - client-public\n      - client-confidential-symmetric\n      - client-confidential-asymmetric\n      - context-banner\n      - context-style\n      - context-ehr-patient\n\
  \      - context-ehr-encounter\n      - context-standalone-patient\n      - permission-offline\n      - permission-patient\n      - permission-user\n      - permission-v1\n      - permission-v2\n      - sso-openid-connect\n      - authorize-post\n    backend_services: true\n    backend_services_evidence: >-\n      private_key_jwt + jwt-bearer grant + a published jwks_uri is the SMART\n      Backend Services (system-level) shape, which is what the Bulk Data export\n      requires.\n    registration: https://fhir.epic.com/Developer/Apps\n    registration_note: >-\n      Client registration is handled by Epic on FHIR, not by Jefferson Health\n      directly; Jefferson approves the app for production against its own\n      endpoint.\n    sources:\n      - well-known/jefferson-health-tjuh-smart-configuration.json\n      - well-known/jefferson-health-tjuh-openid-configuration.json\n      - conformance/jefferson-health-tjuh-fhir-r4-capabilitystatement.json\n      - openapi/_original/jefferson-health-tjuh-fhir-r4-api-openapi.yml\n\
  \n  - name: jhpSmartAuth\n    type: oauth2\n    server: jhp-patient-access\n    applies_to: https://smilercdr.healthpartnersplans.com/\n    required: true\n    description: >-\n      Jefferson Health Plans SMART on FHIR authorization server for the CARIN\n      Blue Button Patient Access API. Developer registration runs through the\n      JHP App Gallery developer portal.\n    issuer: https://appgallery.healthpartnersplans.com/smartauth-fhir\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://appgallery.healthpartnersplans.com/smartauth-fhir/oauth/authorize\n        tokenUrl: https://appgallery.healthpartnersplans.com/smartauth-fhir/oauth/token\n    response_types_supported: [code, code id_token, token, token id_token]\n    code_challenge_methods_supported: [plain, S256]\n    pkce_required: false\n    pkce_note: >-\n      'plain' is advertised alongside S256. Clients should insist on S256; the\n      server permitting 'plain' is a weaker posture than the hospital\
  \ endpoint,\n      which offers S256 only.\n    introspection_endpoint: https://appgallery.healthpartnersplans.com/smartauth-fhir/oauth/token/introspect\n    userinfo_endpoint: https://appgallery.healthpartnersplans.com/smartauth-fhir/userinfo\n    revocation_endpoint: https://appgallery.healthpartnersplans.com/smartauth-fhir/oauth/token/revoke\n    session_management_endpoint: https://appgallery.healthpartnersplans.com/smartauth-fhir/session/management\n    jwks_uri: https://appgallery.healthpartnersplans.com/smartauth-fhir/jwk\n    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported: [public]\n    registration: https://appgallery.healthpartnersplans.com/app-gallery/portal/\n    sources:\n      - well-known/jefferson-health-jhp-openid-configuration.json\n      - conformance/jefferson-health-jhp-provider-directory-capabilitystatement.json\n\n  - name: anonymous\n    type: none\n    server: jhp-provider-directory\n    applies_to: https://providerfhirapi.healthpartnersplans.com\n\
  \    required: false\n    description: >-\n      The Da Vinci Plan-Net provider directory requires no credentials. Verified\n      live: GET /InsurancePlan?_count=1 and GET /Practitioner?_count=2 both\n      returned HTTP 200 searchset Bundles with no Authorization header.\n    note: >-\n      The CapabilityStatement still advertises SMART oauth-uris pointing at the\n      appgallery authorization server, which is a decoy for this host — do not\n      build an auth flow for the directory.\n\nobserved_behaviour:\n  - server: tjuh-fhir-r4\n    request: GET /Patient?family=Smith with no Authorization header\n    http_status: 401\n    content_type: application/json\n    body: '(empty)'\n    note: >-\n      No OperationOutcome and no challenge body. An agent must branch on the\n      status code alone.\n  - server: jhp-provider-directory\n    request: GET /Practitioner?_count=2 with no Authorization header\n    http_status: 200\n    note: Anonymous read confirmed.\n\ngaps:\n  - >-\n    No published\
  \ token lifetime, refresh-token lifetime, or client-credential\n    rotation policy on either authorization server.\n  - >-\n    The Jefferson Health Plans Patient Access SMART configuration is not served:\n    https://smilercdr.healthpartnersplans.com/smartauth/well-known/openid-configuration\n    returns the portal HTML shell (soft 200), and\n    https://appgallery.healthpartnersplans.com/smartauth-fhir/.well-known/smart-configuration\n    likewise. Only the OIDC discovery document is machine-readable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jefferson-health/refs/heads/main/authentication/jefferson-health-authentication.yml
summary_line: oauth2/openIdConnect/none · 3 schemes
tags:
- Academic Medical Center
- CARIN Blue Button
- CMS Interoperability
- Cures Act
- Da Vinci Plan-Net
- Epic
- FHIR
- HL7
- Healthcare
- Hospital System
- MyChart
- OAuth 2.0
- Patient Access
- Provider Directory
- SMART on FHIR
- US Core
- USCDI
---
