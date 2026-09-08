---
anonymous_access: false
api_key_in: []
api_specs:
- filename: elevance-health-claims-api-openapi.yml
  format: yaml
  label: Elevance Health Claims API
  slug: elevance-health-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/openapi/elevance-health-claims-api-openapi.yml
- filename: elevance-health-conformance-api-openapi.yml
  format: yaml
  label: Elevance Health Conformance API
  slug: elevance-health-conformance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/openapi/elevance-health-conformance-api-openapi.yml
- filename: elevance-health-coverage-api-openapi.yml
  format: yaml
  label: Elevance Health Coverage API
  slug: elevance-health-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/openapi/elevance-health-coverage-api-openapi.yml
- filename: elevance-health-patient-api-openapi.yml
  format: yaml
  label: Elevance Health Patient API
  slug: elevance-health-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/openapi/elevance-health-patient-api-openapi.yml
- filename: elevance-health-provider-directory-api-openapi.yml
  format: yaml
  label: Elevance Health Provider Directory API
  slug: elevance-health-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/openapi/elevance-health-provider-directory-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: Elevance Health runs three distinct authorization surfaces across its FHIR estate. Member-facing Patient Access uses SMART on FHIR / OAuth 2.0 authorization code with PKCE and member consent. The public CMS Provider Directory and Formulary APIs use OAuth 2.0 client credentials, with the client id, client secret and token endpoint delivered by secure email after a registration form is approved. The legacy Patient360 (DSTU2) surface uses an IdentityServer-backed SMART/OIDC stack.
kind: authentication
layout: security
mechanism_count: 4
method: probed
name: Elevance Health Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Elevance Health secures its APIs with oauth2 and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Elevance Health
provider_slug: elevance-health
scheme_count: 4
schemes:
- api: Patient Access API (production, CMS Interoperability)
  code_challenge_methods_supported:
  - S256
  discovery: https://totalview.healthos.elevancehealth.com/resources/registered/{Brand}/api/v1/fhir/.well-known/smart-configuration
  flows:
  - authorizationUrl: https://totalview.healthos.elevancehealth.com/oauth2.code/registered/api/v1/authorize
    flow: authorizationCode
    scopes: 67
    tokenUrl: https://totalview.healthos.elevancehealth.com/client.oauth2/registered/api/v1/token
  - flow: clientCredentials
    tokenUrl: https://totalview.healthos.elevancehealth.com/client.oauth2/registered/api/v1/token
  name: patient-access-production
  onboarding: Registration form at https://www.anthem.com/developers/request-anthem-io; production approval can take several weeks.
  smart_capabilities:
  - launch-standalone
  - client-public
  - context-standalone-patient
  - permission-offline
  - permission-patient
  sources:
  - well-known/elevance-health-totalview-smart-configuration.json
  standard: SMART App Launch Framework 2.2.0
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  token_endpoint_auth_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - ES384
  - ES512
  type: oauth2
- api: Provider Directory API and Formulary API (public CMS surfaces)
  data_endpoints:
  - https://totalview.healthos.elevancehealth.com/resources/unregistered/api/v1/fhir/cms_mandate/mcd/
  - https://totalview.healthos.elevancehealth.com/resources/unregistered/api/v1/fhir/cms_mandate/frmlry
  flows:
  - flow: clientCredentials
    note: The token endpoint URL is not published. IO105 v15.0 states it is issued to each registered third-party application by secure email along with the client id and client secret. Requests use grant_type=client_credentials with HTTP Basic authentication of the client credentials.
    tokenUrl: null
  name: provider-directory-and-formulary
  onboarding: Provider Directory API / Formulary API Production Environment request forms on the Anthem developer portal.
  sources:
  - https://www.anthem.com/content/dam/digital/developers-portal/Anthem-IOProviderDirectoryAndFormulary-API-Documentation.pdf
  - conformance/elevance-health-provider-directory-capabilitystatement.json
  type: oauth2
- api: Patient360 FHIR (DSTU2, CareEvolution HIEBus)
  cors: true
  discovery: https://patient360.anthem.com/P360Member/api/fhir/.well-known/smart-configuration
  flows:
  - authorizationUrl: https://patient360c.anthem.com/P360Member/identityserver/connect/authorize
    flow: authorizationCode
    scopes: 205
    tokenUrl: https://patient360c.anthem.com/P360Member/identityserver/connect/token
  introspection_endpoint: https://patient360c.anthem.com/P360Member/api/tokenintrospection
  name: patient360-dstu2
  smart_capabilities:
  - launch-ehr
  - launch-standalone
  - client-public
  - client-confidential-symmetric
  - sso-openid-connect
  - context-banner
  - context-ehr-patient
  - context-standalone-patient
  - permission-offline
  - permission-patient
  - permission-user
  sources:
  - well-known/elevance-health-patient360-smart-configuration.json
  - well-known/elevance-health-patient360c-smart-configuration.json
  - conformance/elevance-health-patient360-dstu2-conformance.xml
  standard: SMART on FHIR (restful-security-service code SMART-on-FHIR in the conformance statement)
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: oauth2
- api: Patient360 IdentityServer
  claims_supported:
  - sub
  - role
  - email
  - email_verified
  - name
  - family_name
  - given_name
  - middle_name
  - nickname
  - preferred_username
  - picture
  - website
  - gender
  - birthdate
  - zoneinfo
  - locale
  - updated_at
  - profile
  - fhirUser
  - patientidentifier
  - participantidentifier
  - verifiedemail
  code_challenge_methods_supported:
  - plain
  - S256
  end_session_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/endsession
  grant_types_supported:
  - authorization_code
  - client_credentials
  - password
  - refresh_token
  - implicit
  - post_login
  - cookie_to_token
  - new_token
  - external_token
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/introspect
  issuer: https://patient360.anthem.com/P360Member/identityserver
  jwks_uri: https://patient360c.anthem.com/P360Member/identityserver/.well-known/jwks
  name: patient360-openid-connect
  openIdConnectUrl: https://patient360c.anthem.com/P360Member/identityserver/.well-known/openid-configuration
  revocation_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/revocation
  scopes_supported_count: 1048
  sources:
  - well-known/elevance-health-patient360c-openid-configuration.json
  type: openIdConnect
  userinfo_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/userinfo
slug: elevance-health-authentication
source_filename: elevance-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  Anonymous GET of the SMART App Launch configurations at\n  https://patient360.anthem.com/P360Member/api/fhir/.well-known/smart-configuration,\n  https://patient360c.anthem.com/P360Member/api/fhir/.well-known/smart-configuration and\n  https://totalview.healthos.elevancehealth.com/resources/registered/AnthemBlueCross/api/v1/fhir/.well-known/smart-configuration,\n  the OpenID Connect discovery document at\n  https://patient360c.anthem.com/P360Member/identityserver/.well-known/openid-configuration,\n  the FHIR conformance/capability statements on each host, and the first-party\n  \"Interoperability API Endpoint Support Document\" (IO105 v15.0, effective 2025-11-18) at\n  https://www.anthem.com/content/dam/digital/developers-portal/Anthem-IOProviderDirectoryAndFormulary-API-Documentation.pdf\ndescription: >-\n  Elevance Health runs three distinct authorization surfaces across its FHIR estate. Member-facing\n  Patient Access\
  \ uses SMART on FHIR / OAuth 2.0 authorization code with PKCE and member consent.\n  The public CMS Provider Directory and Formulary APIs use OAuth 2.0 client credentials, with the\n  client id, client secret and token endpoint delivered by secure email after a registration form\n  is approved. The legacy Patient360 (DSTU2) surface uses an IdentityServer-backed SMART/OIDC stack.\ncorrection: >-\n  Supersedes the 2026-07-11 derived profile, which carried OAuth endpoints\n  (/P360Member/oauth2/authorize, /P360Member/oauth2/token) that do not exist. The real\n  Patient360 endpoints are under /P360Member/identityserver/connect/. The prior values came from a\n  hand-written scaffold spec in openapi/_original/, not from the provider.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  surfaces: 3\n  pkce: S256\n  member_consent_required: true\n  token_lifetime_note: Patient Access production consent tokens are valid for 90 days;\
  \ continued access requires renewed member consent (IO105 v15.0).\nschemes:\n- name: patient-access-production\n  api: Patient Access API (production, CMS Interoperability)\n  type: oauth2\n  standard: SMART App Launch Framework 2.2.0\n  discovery: https://totalview.healthos.elevancehealth.com/resources/registered/{Brand}/api/v1/fhir/.well-known/smart-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://totalview.healthos.elevancehealth.com/oauth2.code/registered/api/v1/authorize\n    tokenUrl: https://totalview.healthos.elevancehealth.com/client.oauth2/registered/api/v1/token\n    scopes: 67\n  - flow: clientCredentials\n    tokenUrl: https://totalview.healthos.elevancehealth.com/client.oauth2/registered/api/v1/token\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  token_endpoint_auth_signing_alg_values_supported: [RS256, RS384, RS512, ES384, ES512]\n  code_challenge_methods_supported: [S256]\n  smart_capabilities:\n\
  \  - launch-standalone\n  - client-public\n  - context-standalone-patient\n  - permission-offline\n  - permission-patient\n  onboarding: Registration form at https://www.anthem.com/developers/request-anthem-io; production approval can take several weeks.\n  sources:\n  - well-known/elevance-health-totalview-smart-configuration.json\n- name: provider-directory-and-formulary\n  api: Provider Directory API and Formulary API (public CMS surfaces)\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: null\n    note: >-\n      The token endpoint URL is not published. IO105 v15.0 states it is issued to each registered\n      third-party application by secure email along with the client id and client secret. Requests\n      use grant_type=client_credentials with HTTP Basic authentication of the client credentials.\n  data_endpoints:\n  - https://totalview.healthos.elevancehealth.com/resources/unregistered/api/v1/fhir/cms_mandate/mcd/\n  - https://totalview.healthos.elevancehealth.com/resources/unregistered/api/v1/fhir/cms_mandate/frmlry\n\
  \  onboarding: Provider Directory API / Formulary API Production Environment request forms on the Anthem developer portal.\n  sources:\n  - https://www.anthem.com/content/dam/digital/developers-portal/Anthem-IOProviderDirectoryAndFormulary-API-Documentation.pdf\n  - conformance/elevance-health-provider-directory-capabilitystatement.json\n- name: patient360-dstu2\n  api: Patient360 FHIR (DSTU2, CareEvolution HIEBus)\n  type: oauth2\n  standard: SMART on FHIR (restful-security-service code SMART-on-FHIR in the conformance statement)\n  discovery: https://patient360.anthem.com/P360Member/api/fhir/.well-known/smart-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://patient360c.anthem.com/P360Member/identityserver/connect/authorize\n    tokenUrl: https://patient360c.anthem.com/P360Member/identityserver/connect/token\n    scopes: 205\n  introspection_endpoint: https://patient360c.anthem.com/P360Member/api/tokenintrospection\n  token_endpoint_auth_methods:\n \
  \ - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  smart_capabilities:\n  - launch-ehr\n  - launch-standalone\n  - client-public\n  - client-confidential-symmetric\n  - sso-openid-connect\n  - context-banner\n  - context-ehr-patient\n  - context-standalone-patient\n  - permission-offline\n  - permission-patient\n  - permission-user\n  cors: true\n  sources:\n  - well-known/elevance-health-patient360-smart-configuration.json\n  - well-known/elevance-health-patient360c-smart-configuration.json\n  - conformance/elevance-health-patient360-dstu2-conformance.xml\n- name: patient360-openid-connect\n  api: Patient360 IdentityServer\n  type: openIdConnect\n  openIdConnectUrl: https://patient360c.anthem.com/P360Member/identityserver/.well-known/openid-configuration\n  issuer: https://patient360.anthem.com/P360Member/identityserver\n  jwks_uri: https://patient360c.anthem.com/P360Member/identityserver/.well-known/jwks\n  userinfo_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/userinfo\n\
  \  revocation_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/revocation\n  introspection_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/introspect\n  end_session_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/endsession\n  grant_types_supported: [authorization_code, client_credentials, password, refresh_token, implicit, post_login, cookie_to_token, new_token, external_token]\n  id_token_signing_alg_values_supported: [RS256]\n  code_challenge_methods_supported: [plain, S256]\n  claims_supported: [sub, role, email, email_verified, name, family_name, given_name, middle_name, nickname, preferred_username, picture, website, gender, birthdate, zoneinfo, locale, updated_at, profile, fhirUser, patientidentifier, participantidentifier, verifiedemail]\n  scopes_supported_count: 1048\n  sources:\n  - well-known/elevance-health-patient360c-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elevance-health/refs/heads/main/authentication/elevance-health-authentication.yml
summary_line: oauth2/openIdConnect · 4 schemes
tags:
- Fortune 500
- Healthcare
- Health Insurance
- FHIR
- Interoperability
- CMS Interoperability
- SMART on FHIR
- Da Vinci PDEX
- CARIN Blue Button
- Payer
- Provider Directory
- Formulary
- HL7
---
