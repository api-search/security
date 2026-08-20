---
api_key_in: []
api_specs:
- filename: temple-health-allergy-intolerance-api-openapi.yml
  format: yaml
  label: Temple Health Allergy Intolerance API
  slug: temple-health-allergy-intolerance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-allergy-intolerance-api-openapi.yml
- filename: temple-health-bulk-data-api-openapi.yml
  format: yaml
  label: Temple Health Bulk Data API
  slug: temple-health-bulk-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-bulk-data-api-openapi.yml
- filename: temple-health-condition-api-openapi.yml
  format: yaml
  label: Temple Health Condition API
  slug: temple-health-condition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-condition-api-openapi.yml
- filename: temple-health-document-reference-api-openapi.yml
  format: yaml
  label: Temple Health Document Reference API
  slug: temple-health-document-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-document-reference-api-openapi.yml
- filename: temple-health-encounter-api-openapi.yml
  format: yaml
  label: Temple Health Encounter API
  slug: temple-health-encounter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-encounter-api-openapi.yml
- filename: temple-health-medication-request-api-openapi.yml
  format: yaml
  label: Temple Health Medication Request API
  slug: temple-health-medication-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-medication-request-api-openapi.yml
- filename: temple-health-metadata-api-openapi.yml
  format: yaml
  label: Temple Health Metadata API
  slug: temple-health-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-metadata-api-openapi.yml
- filename: temple-health-observation-api-openapi.yml
  format: yaml
  label: Temple Health Observation API
  slug: temple-health-observation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-observation-api-openapi.yml
- filename: temple-health-patient-api-openapi.yml
  format: yaml
  label: Temple Health Patient API
  slug: temple-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/openapi/temple-health-patient-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Temple Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- jwtBearer
- tokenExchange
overview: Temple Health secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, jwtBearer, and tokenExchange flow(s).
provider_name: Temple Health
provider_slug: temple-health
scheme_count: 1
schemes:
- description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.
  flows:
  - authorizationUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize
    flow: authorizationCode
    scopes: 13
    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token
  name: smartOnFhir
  sources:
  - openapi/temple-health-allergy-intolerance-api-openapi.yml
  - openapi/temple-health-bulk-data-api-openapi.yml
  - openapi/temple-health-condition-api-openapi.yml
  - openapi/temple-health-document-reference-api-openapi.yml
  - openapi/temple-health-encounter-api-openapi.yml
  - openapi/temple-health-medication-request-api-openapi.yml
  - openapi/temple-health-metadata-api-openapi.yml
  - openapi/temple-health-observation-api-openapi.yml
  - openapi/temple-health-patient-api-openapi.yml
  type: oauth2
slug: temple-health-authentication
source_filename: temple-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: Live GET of the SMART configuration, the OIDC discovery document and the JWKS on epicaccess.templehealth.org\n  (all HTTP 200, 2026-08-15), plus an observed 401 challenge on GET /FHIR/R4/Patient/example. Reconciled\n  against the oauth2 securityScheme in openapi/*.yml.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\n  - jwtBearer\n  - tokenExchange\n  pkce: S256 (only method supported)\n  client_auth:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  bearer_challenge: 'WWW-Authenticate: Bearer (observed on 401; no realm, no resource_metadata)'\n  anonymous_endpoints:\n  - /FHIR/R4/metadata\n  - /FHIR/R4/.well-known/smart-configuration\n  - /FHIR/DSTU2/metadata\n  - /FhirProxyPrd/oauth2/.well-known/openid-configuration\nschemes:\n- name: smartOnFhir\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/authorize\n    tokenUrl: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/token\n    scopes: 13\n  description: SMART on FHIR / OAuth 2.0 with PKCE for patient-facing and provider-facing app launches.\n  sources:\n  - openapi/temple-health-allergy-intolerance-api-openapi.yml\n  - openapi/temple-health-bulk-data-api-openapi.yml\n  - openapi/temple-health-condition-api-openapi.yml\n  - openapi/temple-health-document-reference-api-openapi.yml\n  - openapi/temple-health-encounter-api-openapi.yml\n  - openapi/temple-health-medication-request-api-openapi.yml\n  - openapi/temple-health-metadata-api-openapi.yml\n  - openapi/temple-health-observation-api-openapi.yml\n  - openapi/temple-health-patient-api-openapi.yml\ndocs: https://fhir.epic.com/Documentation\ndocs_note: There is no Temple Health-authored authentication page. Epic on FHIR documents the SMART/OAuth\n  model generally; the Temple-specific facts come only from the endpoint.\n\
  discovery:\n  smart_configuration:\n    url: https://epicaccess.templehealth.org/FhirProxyPrd/api/FHIR/R4/.well-known/smart-configuration\n    status: 200\n    file: well-known/temple-health-smart-configuration.json\n  openid_configuration:\n    url: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2/.well-known/openid-configuration\n    status: 200\n    file: well-known/temple-health-openid-configuration.json\n  jwks:\n    url: https://epicaccess.templehealth.org/FhirProxyPrd/api/epic/2019/Security/Open/PublicKeys/530027/OIDC\n    status: 200\n    file: well-known/temple-health-oidc-jwks.json\n  oauth_authorization_server_rfc8414:\n    status: 404\n  oauth_protected_resource_rfc9728:\n    status: 404\n  dstu2_smart_configuration:\n    status: 404\n    note: The legacy DSTU2 base publishes no SMART discovery document; read the oauth-uris extension from\n      its Conformance resource instead.\nopenid_connect:\n  issuer: https://epicaccess.templehealth.org/FhirProxyPrd/oauth2\n  id_token_signing_alg_values_supported:\n\
  \  - RS256\n  subject_types_supported:\n  - public\n  response_types_supported:\n  - code\n  response_modes_supported:\n  - query\nprofiles:\n- name: SMART App Launch — standalone patient\n  grant: authorization_code + PKCE S256\n  client: public or confidential\n  use: Patient-access apps under CMS-9115-F\n  capability_evidence:\n  - launch-standalone\n  - context-standalone-patient\n  - permission-patient\n  - permission-offline\n- name: SMART App Launch — EHR launch\n  grant: authorization_code + PKCE S256\n  client: confidential\n  use: Provider-facing apps launched from inside Epic\n  capability_evidence:\n  - launch-ehr\n  - context-ehr-patient\n  - context-ehr-encounter\n  - permission-user\n- name: SMART Backend Services\n  grant: client_credentials with private_key_jwt (RFC 7523)\n  client: confidential-asymmetric\n  use: Bulk Data Group $export under a data-use agreement\n  capability_evidence:\n  - client-confidential-asymmetric\nonboarding:\n  app_registration: https://fhir.epic.com/Developer/Apps\n\
  \  production_access: Approved by Temple Health per app against the production endpoint; no self-service\n    path.\n  endpoint_directory: https://open.epic.com/Endpoints/R4\ngaps:\n- No RFC 9728 protected-resource metadata — the 401 challenge carries no pointer to the authorization\n  server.\n- No RFC 8414 authorization-server metadata at either the origin root or the FHIR base.\n- The 401 body is an empty JSON string, not an OperationOutcome — no machine-readable reason for the rejection.\n- No dynamic client registration endpoint published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temple-health/refs/heads/main/authentication/temple-health-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Academic Medical Center
- CMS Interoperability
- Cures Act
- DSTU2
- Epic
- FHIR
- Fox Chase Cancer Center
- HL7
- Healthcare
- Hospital System
- MyChart
- Authentication
- Patient Access
- Price Transparency
- R4
- SMART on FHIR
- Temple University
- US Core
- USCDI
---
