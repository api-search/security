---
api_key_in: []
api_specs:
- filename: independence-blue-cross-formulary-api-openapi.yml
  format: yaml
  label: Independence Blue Cross Formulary API
  slug: independence-blue-cross-formulary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/openapi/independence-blue-cross-formulary-api-openapi.yml
- filename: independence-blue-cross-patient-access-api-openapi.yml
  format: yaml
  label: Independence Blue Cross Patient Access API
  slug: independence-blue-cross-patient-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/openapi/independence-blue-cross-patient-access-api-openapi.yml
- filename: independence-blue-cross-provider-directory-api-openapi.yml
  format: yaml
  label: Independence Blue Cross Provider Directory API
  slug: independence-blue-cross-provider-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/openapi/independence-blue-cross-provider-directory-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Independence Blue Cross Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Independence Blue Cross secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Independence Blue Cross
provider_slug: independence-blue-cross
scheme_count: 2
schemes:
- applies_to: Independence Blue Cross Patient Access API
  base: https://eapics.ibx.com/patient/v1/fhir
  cross_link: scopes/independence-blue-cross-scopes.yml
  flows:
  - authorizationUrl: https://member.ibx.com/patientaccesssvc/oauth2/v1/authorize
    flow: authorizationCode
    pkce: required-for-public-clients
    scope_list:
    - launch/patient
    - patient/*.read
    - openid
    - offline_access
    scopes: 4
    tokenUrl: https://eapics.ibx.com/oauth2/v2/token
  name: smart_on_fhir
  profile: SMART App Launch 1.0.0
  sources:
  - openapi/_original/independence-blue-cross-patient-openapi.yml
  - https://eapics.ibx.com/patient/v1/fhir/.well-known/smart-configuration
  token_placement: 'Authorization: Bearer {access_token}'
  type: oauth2
- applies_to:
  - Independence Blue Cross Provider Directory API
  - Independence Blue Cross Drug Formulary API
  bases:
  - https://eapics.ibx.com/provider/v1/fhir
  - https://eapics.ibx.com/formulary/v1/fhir
  evidence: Provider Swagger info.description; confirmed by openapi/_original/independence-blue-cross-provider-openapi.yml and openapi/_original/independence-blue-cross-formulary-openapi.yml declaring no securitySchemes.
  name: public
  type: none
slug: independence-blue-cross-authentication
source_filename: independence-blue-cross-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: probed\nsource: >-\n  https://eapics.ibx.com/patient/v1/fhir/.well-known/smart-configuration (HTTP 200, live probe 2026-08-15),\n  https://eapics.ibx.com/provider/v1/fhir/.well-known/smart-configuration (HTTP 200),\n  https://eapics.ibx.com/formulary/v1/fhir/.well-known/smart-configuration (HTTP 200),\n  https://www.ibx.com/scripts/custom/swagger/cmsSwagger.json (provider-published Swagger 2.0),\n  openapi/_original/independence-blue-cross-patient-openapi.yml,\n  https://www.ibx.com/htdocs/custom/tnc/Developer%20Portal%20TandC.pdf\ndocs: https://www.ibx.com/developer-resources/index.html\nprevious_method: derived\nupgrade_note: >-\n  Upgraded from derived to probed. The 2026-07-11 pass read the auth model out of the OpenAPI alone;\n  this pass fetched the live SMART App Launch configuration from all three FHIR base paths and\n  reconciled it against the provider's own published Swagger description. The endpoints agree, and the\n  live documents\
  \ add the capability set, which the spec does not carry.\nsummary:\n  types:\n    - oauth2\n  oauth2_flows:\n    - authorizationCode\n  profile: SMART App Launch 1.0.0\n  split_surface: true\n  split_note: >-\n    Only one of the three Independence Blue Cross APIs is authenticated. Patient Access requires SMART\n    on FHIR OAuth 2.0 with member consent; the Provider Directory and Drug Formulary require nothing at\n    all. The provider states this plainly in its Swagger info.description: those two APIs \"do not\n    require authorization to access the data on the server, because customer data is not being shared.\"\nschemes:\n  - name: smart_on_fhir\n    type: oauth2\n    profile: SMART App Launch 1.0.0\n    applies_to: Independence Blue Cross Patient Access API\n    base: https://eapics.ibx.com/patient/v1/fhir\n    token_placement: 'Authorization: Bearer {access_token}'\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://member.ibx.com/patientaccesssvc/oauth2/v1/authorize\n\
  \        tokenUrl: https://eapics.ibx.com/oauth2/v2/token\n        pkce: required-for-public-clients\n        scopes: 4\n        scope_list:\n          - launch/patient\n          - patient/*.read\n          - openid\n          - offline_access\n    sources:\n      - openapi/_original/independence-blue-cross-patient-openapi.yml\n      - https://eapics.ibx.com/patient/v1/fhir/.well-known/smart-configuration\n    cross_link: scopes/independence-blue-cross-scopes.yml\n  - name: public\n    type: none\n    applies_to:\n      - Independence Blue Cross Provider Directory API\n      - Independence Blue Cross Drug Formulary API\n    bases:\n      - https://eapics.ibx.com/provider/v1/fhir\n      - https://eapics.ibx.com/formulary/v1/fhir\n    evidence: >-\n      Provider Swagger info.description; confirmed by openapi/_original/independence-blue-cross-provider-openapi.yml\n      and openapi/_original/independence-blue-cross-formulary-openapi.yml declaring no securitySchemes.\nsmart_configuration:\n\
  \  discovery_pattern: '{base}/.well-known/smart-configuration'\n  probed: '2026-08-15'\n  documents:\n    - base: https://eapics.ibx.com/patient/v1/fhir\n      status: 200\n      authorization_endpoint: https://member.ibx.com/patientaccesssvc/oauth2/v1/authorize\n      token_endpoint: https://eapics.ibx.com/oauth2/v2/token\n      file: well-known/independence-blue-cross-patient-smart-configuration.json\n    - base: https://eapics.ibx.com/provider/v1/fhir\n      status: 200\n      authorization_endpoint: https://member.ibx.com/patientaccesssvc/oauth2/v1/authorize\n      token_endpoint: https://eapics.ibx.com/oauth2/v2/token\n      file: well-known/independence-blue-cross-provider-smart-configuration.json\n    - base: https://eapics.ibx.com/formulary/v1/fhir\n      status: 200\n      authorization_endpoint: https://member.amerihealth.com/patientaccesssvc/oauth2/v1/authorize\n      token_endpoint: https://eapics.amerihealth.com/oauth2/v1/token\n      file: well-known/independence-blue-cross-formulary-smart-configuration.json\n\
  \      deviation: >-\n        Cross-brand. This document is served from an ibx.com host but names AmeriHealth authorization\n        and token endpoints. AmeriHealth is a sibling payer under the same parent, Independence Health\n        Group, Inc., and the two evidently share one FHIR platform. Recorded verbatim as served. It has\n        no practical effect because the formulary API is unauthenticated, but a client that blindly\n        followed SMART discovery from this base would authenticate against the wrong brand.\n  capabilities:\n    - client-public\n    - sso-openid-connect\n    - launch-standalone\n    - client-confidential-symmetric\n    - context-standalone-patient\n    - permission-offline\n    - permission-patient\n  capability_reading: >-\n    client-public plus client-confidential-symmetric means both public (PKCE-protected) and\n    confidential (shared-secret) clients are supported. launch-standalone plus\n    context-standalone-patient means standalone launch with a\
  \ single patient context — there is no EHR\n    launch. permission-offline confirms refresh tokens via offline_access. permission-patient confirms\n    patient/*.* scopes. There is no permission-user and no permission-system, so there is no\n    provider-facing or backend-services (SMART Backend Services / client_credentials) surface.\n  absent:\n    - registration_endpoint      # no dynamic client registration\n    - introspection_endpoint\n    - revocation_endpoint\n    - grant_types_supported\n    - scopes_supported\n    - code_challenge_methods_supported\n  absent_note: >-\n    The three documents carry only authorization_endpoint, token_endpoint and capabilities. SMART App\n    Launch treats several of the missing fields as recommended, so this is a thin discovery document\n    even by its own specification.\ntoken_lifetime:\n  published: false\n  note: >-\n    Neither the smart-configuration documents nor any public page states an access-token lifetime.\n    Request offline_access\
  \ and refresh on a 401 rather than on an assumed expiry.\nregistration:\n  url: https://devportal.ibx.com/cmssignin/\n  process: >-\n    Register the company and each member-facing application in the developer portal, then activate the\n    account. Credentials are issued per registered application. Developer Portal Terms section 3: IBC\n    may revoke credentials used with an application or product not registered with IBC.\n  support: mailto:AppOnboardingSupport@ibx.com\n  gated: true\n  gated_note: >-\n    devportal.ibx.com renders entirely in JavaScript and returns no readable content to a non-executing\n    client, so the post-registration auth documentation could not be read by this pass.\noidc_discovery:\n  served: false\n  probed:\n    - url: https://eapics.ibx.com/.well-known/openid-configuration\n      status: 404\n    - url: https://eapics.ibx.com/patient/v1/fhir/.well-known/openid-configuration\n      status: 404\n    - url: https://eapics.ibx.com/.well-known/oauth-authorization-server\n\
  \      status: 404\n    - url: https://eapics.ibx.com/patient/v1/fhir/.well-known/oauth-authorization-server\n      status: 404\n    - url: https://eapics.ibx.com/patient/v1/fhir/.well-known/oauth-protected-resource\n      status: 404\n  note: >-\n    The sso-openid-connect capability is advertised but no OIDC discovery document and no RFC 8414\n    authorization-server metadata is served anywhere. member.ibx.com — which hosts the authorization\n    endpoint — returns 403 to every anonymous request, so its metadata could not be probed either.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/independence-blue-cross/refs/heads/main/authentication/independence-blue-cross-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Healthcare
- Health Insurance
- Blue Cross Blue Shield
- Managed Care
- Medicare
- Medicare Advantage
- Medicaid
- CHIP
- Commercial
- Dental
- Vision
- Behavioral Health
- Pharmacy Benefits
- Interoperability
- FHIR
- SMART On FHIR
- CMS
- Patient Access
- Provider Directory
- Drug Formulary
- Transparency In Coverage
---
