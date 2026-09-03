---
api_key_in: []
api_specs:
- filename: anthem-provider-directory-api-openapi.yml
  format: yaml
  label: Anthem Provider Directory API
  slug: provider-directory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthem/refs/heads/main/openapi/anthem-provider-directory-api-openapi.yml
- filename: anthem-drug-formulary-api-openapi.yml
  format: yaml
  label: Anthem Drug Formulary API
  slug: drug-formulary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthem/refs/heads/main/openapi/anthem-drug-formulary-api-openapi.yml
- filename: anthem-patient360-member-fhir-api-openapi.yml
  format: yaml
  label: Anthem Patient360 Member FHIR API
  slug: patient360-member-fhir
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anthem/refs/heads/main/openapi/anthem-patient360-member-fhir-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Anthem Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Anthem secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Anthem
provider_slug: anthem
scheme_count: 2
schemes:
- code_challenge_methods_supported:
  - plain
  - S256
  description: SMART on FHIR authorization, declared by the FHIR server's own security extension http://fhir-registry.smarthealthit.org/StructureDefinition/oauth-uris in its live Conformance statement, and corroborated by the identity server's OpenID Connect discovery document.
  end_session_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/endsession
  flows:
  - authorizationUrl: https://patient360c.anthem.com/P360Member/identityserver/connect/authorize
    flow: authorizationCode
    refreshUrl: https://patient360c.anthem.com/P360Member/identityserver/connect/token
    scopes: 1048
    tokenUrl: https://patient360c.anthem.com/P360Member/identityserver/connect/token
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
  method: probed
  name: smartOnFhir
  pkce: true
  platform: Patient360 member FHIR (patient360c.anthem.com)
  revocation_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/revocation
  sources:
  - https://patient360c.anthem.com/P360Member/api/fhir/metadata
  - https://patient360c.anthem.com/P360Member/identityserver/.well-known/openid-configuration
  - openapi/anthem-patient360-member-fhir-api-openapi.yml
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  type: oauth2
  userinfo_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/userinfo
- credential_issuance: 'Complete the Provider Directory API or Formulary API Production Environment request form on the developer portal. On approval Anthem sends the client id, client secret and access token URL by secure email. Token requests are POSTed with Content-Type application/x-www-form-urlencoded, HTTP Basic authorization carrying the base64 client id:secret, and grant_type=client_credentials. API calls then carry Authorization: Bearer <token>.'
  description: OAuth 2.0 client-credentials bearer token for the Provider Directory and Formulary APIs.
  method: searched
  name: bearerAuth
  oauth2_flow: clientCredentials
  platform: CMS-mandate FHIR (totalview.healthos.elevancehealth.com)
  scheme: bearer
  sources:
  - https://www.anthem.com/content/dam/digital/developers-portal/Anthem-IOProviderDirectoryAndFormulary-API-Documentation.pdf
  - openapi/anthem-provider-directory-api-openapi.yml
  - openapi/anthem-drug-formulary-api-openapi.yml
  token_endpoint: issued to each approved developer by secure email; not published
  type: http
slug: anthem-authentication
source_filename: anthem-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://www.anthem.com/content/dam/digital/developers-portal/Anthem-IOProviderDirectoryAndFormulary-API-Documentation.pdf\ndocs: https://www.anthem.com/developers\nnote: >-\n  Anthem runs two distinct authorization models across two distinct API platforms, and they do not share\n  an identity provider. (1) The CMS-mandate APIs on totalview.healthos.elevancehealth.com use OAuth 2.0\n  CLIENT CREDENTIALS: Anthem issues the client id, the client secret AND the token endpoint URL itself\n  over secure email once a Production Environment request form is approved, so there is no published\n  token endpoint and no discovery document for that platform. (2) The Patient360 member FHIR server on\n  patient360c.anthem.com uses SMART on FHIR / OpenID Connect authorization_code, and its identity server\n  publishes a full anonymous discovery document with 1,048 scopes. Endpoints below marked probed were read\n  from that live document on\
  \ 2026-09-02; endpoints for platform (1) are documented as issued-by-email\n  because Anthem publishes no URL for them.\nsummary:\n  types:\n    - oauth2\n    - http\n  oauth2_flows:\n    - authorizationCode\n    - clientCredentials\n  member_consent_required: true\n  token_lifetime: >-\n    Patient Access production tokens are valid for 90 days; continued access requires renewed member\n    consent (Anthem Interoperability API Endpoint Support Document IO105 v15.0).\nschemes:\n  - name: smartOnFhir\n    type: oauth2\n    platform: Patient360 member FHIR (patient360c.anthem.com)\n    method: probed\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://patient360c.anthem.com/P360Member/identityserver/connect/authorize\n        tokenUrl: https://patient360c.anthem.com/P360Member/identityserver/connect/token\n        refreshUrl: https://patient360c.anthem.com/P360Member/identityserver/connect/token\n        scopes: 1048\n    issuer: https://patient360.anthem.com/P360Member/identityserver\n\
  \    jwks_uri: https://patient360c.anthem.com/P360Member/identityserver/.well-known/jwks\n    introspection_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/introspect\n    revocation_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/revocation\n    userinfo_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/userinfo\n    end_session_endpoint: https://patient360c.anthem.com/P360Member/identityserver/connect/endsession\n    pkce: true\n    code_challenge_methods_supported: [plain, S256]\n    id_token_signing_alg_values_supported: [RS256]\n    token_endpoint_auth_methods_supported: [client_secret_post, client_secret_basic]\n    grant_types_supported:\n      - authorization_code\n      - client_credentials\n      - password\n      - refresh_token\n      - implicit\n      - post_login\n      - cookie_to_token\n      - new_token\n      - external_token\n    description: >-\n      SMART on FHIR authorization, declared\
  \ by the FHIR server's own security extension\n      http://fhir-registry.smarthealthit.org/StructureDefinition/oauth-uris in its live Conformance\n      statement, and corroborated by the identity server's OpenID Connect discovery document.\n    sources:\n      - https://patient360c.anthem.com/P360Member/api/fhir/metadata\n      - https://patient360c.anthem.com/P360Member/identityserver/.well-known/openid-configuration\n      - openapi/anthem-patient360-member-fhir-api-openapi.yml\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    platform: CMS-mandate FHIR (totalview.healthos.elevancehealth.com)\n    method: searched\n    oauth2_flow: clientCredentials\n    token_endpoint: issued to each approved developer by secure email; not published\n    credential_issuance: >-\n      Complete the Provider Directory API or Formulary API Production Environment request form on the\n      developer portal. On approval Anthem sends the client id, client secret and access token URL by\n  \
  \    secure email. Token requests are POSTed with Content-Type application/x-www-form-urlencoded, HTTP\n      Basic authorization carrying the base64 client id:secret, and grant_type=client_credentials. API\n      calls then carry Authorization: Bearer <token>.\n    description: >-\n      OAuth 2.0 client-credentials bearer token for the Provider Directory and Formulary APIs.\n    sources:\n      - https://www.anthem.com/content/dam/digital/developers-portal/Anthem-IOProviderDirectoryAndFormulary-API-Documentation.pdf\n      - openapi/anthem-provider-directory-api-openapi.yml\n      - openapi/anthem-drug-formulary-api-openapi.yml\nregistration:\n  - name: Patient Access API production access\n    url: https://www.anthem.com/developers/request-anthem-io\n    requires: member consent; approval can take several weeks\n  - name: Provider Directory API production access\n    url: https://www.anthem.com/developers/provider-directory-api-request\n    requires: registration form; credentials returned\
  \ by secure email\n  - name: Patient Access sandbox\n    url: https://www.anthem.com/developers\n    requires: developer self-registration; synthetic data only\ncontact: interoperabilityworkgroup@anthem.com\nobservations:\n  - probe: GET https://totalview.healthos.elevancehealth.com/resources/unregistered/api/v1/fhir/cms_mandate/mcd/metadata\n    status: 200\n    note: CapabilityStatement is served anonymously; it declares NO security block at all.\n  - probe: GET https://totalview.healthos.elevancehealth.com/resources/unregistered/api/v1/fhir/cms_mandate/mcd/InsurancePlan\n    status: 500\n    note: >-\n      Anonymous data requests return HTTP 500 with a non-FHIR envelope rather than 401 with a\n      WWW-Authenticate challenge, so a client cannot tell an auth failure from an outage.\n  - probe: GET https://totalview.healthos.elevancehealth.com/resources/unregistered/api/v1/fhir/cms_mandate/frmlry/metadata\n    status: 403\n    note: The Formulary server refuses even its own capability\
  \ statement anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anthem/refs/heads/main/authentication/anthem-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Blue Cross Blue Shield
- CARIN Blue Button
- CMS Interoperability
- Da Vinci PDEX
- Drug Formulary
- FHIR
- Fortune 100
- Health Benefits
- Health Insurance
- Healthcare
- Interoperability
- Patient Access
- Provider Directory
- SMART on FHIR
---
