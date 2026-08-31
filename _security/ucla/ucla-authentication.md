---
api_key_in: []
api_specs:
- filename: ucla-class-sections-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Class Sections API
  slug: ucla-class-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-class-sections-api-openapi.yml
- filename: ucla-classes-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Classes API
  slug: ucla-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-classes-api-openapi.yml
- filename: ucla-courses-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Courses API
  slug: ucla-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-courses-api-openapi.yml
- filename: ucla-dictionary-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Dictionary API
  slug: ucla-dictionary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-dictionary-api-openapi.yml
- filename: ucla-ge-foundations-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles GE Foundations API
  slug: ucla-ge-foundations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-ge-foundations-api-openapi.yml
- filename: ucla-infrastructure-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Infrastructure API
  slug: ucla-infrastructure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-infrastructure-api-openapi.yml
- filename: ucla-myucla-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles My UCLA API
  slug: ucla-myucla-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-myucla-api-openapi.yml
- filename: ucla-production-calendar-jobs-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Production Calendar Jobs API
  slug: ucla-production-calendar-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-production-calendar-jobs-api-openapi.yml
- filename: ucla-weather-api-openapi.yml
  format: yaml
  label: University of California, Los Angeles Weather API
  slug: ucla-weather-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/openapi/ucla-weather-api-openapi.yml
auth_types: []
description: 'Authentication posture across every UCLA surface reachable from the open internet. UCLA is unusual for this cohort: it runs a real, centrally governed API program with one gateway, one documented credential model and one authorization server, all under ucla.edu. What it does not run is a self-service path — every credential is issued by request through the developer portal, and the portal itself signs in through the campus Shibboleth IdP.'
kind: authentication
layout: security
method: probed
name: Ucla Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of California, Los Angeles declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: University of California, Los Angeles
provider_slug: ucla
scheme_count: 4
schemes:
- credential_issuance: App Key and App Secret, issued after an access request is approved in the developer portal. Developers create an App, choose one or more API Products, and the owning campus unit approves. There is no public or dynamic client registration.
  declared_in:
  - openapi/_original/ucla-sis-classes-openapi.yml
  - openapi/_original/ucla-sis-courses-openapi.yml
  - openapi/_original/ucla-sis-dictionary-openapi.yml
  - openapi/_original/ucla-sis-production-calendar-jobs-openapi.yml
  - openapi/_original/ucla-sis-verify-connectivity-openapi.yml
  - openapi/_original/ucla-myucla-menu-data-openapi.yml
  discovery_document: none
  flow: application
  gateway: Google Apigee Edge (api.ucla.edu CNAMEs to ucla-prod.apigee.net)
  name: UCLA API Gateway OAuth 2.0 (client credentials)
  notes: The contracts declare only `read` and `write` as scopes, across all six SIS products. There is no per-product or per-resource scope, so an approved credential is coarse by design and the real access boundary is the API Product an app is subscribed to, not the token scope.
  observed_enforcement: 'HTTP 401 with {"fault":{"faultstring":"Invalid access token","detail":{"errorcode": "oauth.v2.InvalidAccessToken"}}} on a documented SIS route with no token present.'
  pkce_advertised: false
  scopes:
  - read
  - write
  token_endpoint: https://api.ucla.edu/oauth/client_credential/accesstoken?grant_type=client_credentials
  type: oauth2
  x-operator: institution
- declared_in:
  - openapi/_original/ucla-weather-openapi.yml
  in: header
  name: UCLA API Gateway API key (header)
  notes: The UCLA Weather contract is the only one of the seven that uses a header API key rather than OAuth 2.0, and the only one written in OpenAPI 3.0.3 rather than Swagger 2.0. Two credential models on one gateway is an inconsistency worth flagging, not a defect in either.
  observed_enforcement: HTTP 401 on https://api.ucla.edu/weather/api with no key present.
  parameter: x-apikey
  type: apiKey
  x-operator: institution
- assurance_certification:
  - https://refeds.org/sirtfi
  attribute_authority:
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP
    location: https://shb.ais.ucla.edu:8443/shibboleth-idp/profile/SAML2/SOAP/AttributeQuery
  - binding: urn:oasis:names:tc:SAML:1.0:bindings:SOAP-binding
    location: https://shb.ais.ucla.edu:8443/shibboleth-idp/profile/SAML1/SOAP/AttributeQuery
  entity_categories:
  - http://id.incommon.org/category/research-and-scholarship
  - http://refeds.org/category/research-and-scholarship
  - http://id.incommon.org/category/registered-by-incommon
  entity_id: urn:mace:incommon:ucla.edu
  metadata_url: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aucla.edu
  name: UCLA Shibboleth identity provider (SAML 2.0 / SAML 1.1)
  notes: This is the credential every UCLA human authentication path ultimately terminates at, including sign-in to the developer portal itself (/saml_login). It is machine-readable, signed, and federated into eduGAIN through InCommon — the single most under-catalogued institution-operated API surface class in higher education.
  registration_authority: https://incommon.org
  scope: ucla.edu
  security_contact: security@it.ucla.edu
  sso_endpoints:
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
    location: https://shb.ais.ucla.edu/shibboleth-idp/profile/SAML2/POST/SSO
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
    location: https://shb.ais.ucla.edu/shibboleth-idp/profile/SAML2/Redirect/SSO
  - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest
    location: https://shb.ais.ucla.edu/shibboleth-idp/profile/Shibboleth/SSO
  type: saml
  x-operator: institution
- name: BruinLearn (Canvas) OAuth 2.0 and LTI 1.3
  notes: UCLA's students and courses, Instructure's authorization server and contract. Recorded as a relationship; no Canvas contract is saved under this institution.
  observed_enforcement: HTTP 401 {"status":"unauthenticated","errors":[{"message":"user authorization required"}]} on https://bruinlearn.ucla.edu/api/v1/accounts.
  public_metadata: https://bruinlearn.ucla.edu/api/lti/security/jwks
  type: oauth2
  x-operator: tenant
slug: ucla-authentication
source_filename: ucla-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  securityDefinitions read verbatim from the seven OpenAPI documents UCLA publishes at\n  https://developer.api.ucla.edu/sites/default/files/apidoc_specs/ (all HTTP 200);\n  https://api.ucla.edu/sis/dictionary/buildings/v1 (401, Apigee OAuth fault);\n  https://api.ucla.edu/oauth/client_credential/accesstoken (200);\n  https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aucla.edu (200, signed SAML metadata);\n  https://bruinlearn.ucla.edu/api/v1/accounts (401) — all fetched 2026-08-19\nprovider: University of California, Los Angeles\nproviderId: ucla\ndescription: >-\n  Authentication posture across every UCLA surface reachable from the open internet. UCLA is\n  unusual for this cohort: it runs a real, centrally governed API program with one gateway, one\n  documented credential model and one authorization server, all under ucla.edu. What it does\n  not run is a self-service path — every credential is issued by request\
  \ through the developer\n  portal, and the portal itself signs in through the campus Shibboleth IdP.\nschemes:\n- name: UCLA API Gateway OAuth 2.0 (client credentials)\n  type: oauth2\n  x-operator: institution\n  flow: application\n  token_endpoint: https://api.ucla.edu/oauth/client_credential/accesstoken?grant_type=client_credentials\n  gateway: Google Apigee Edge (api.ucla.edu CNAMEs to ucla-prod.apigee.net)\n  declared_in:\n  - openapi/_original/ucla-sis-classes-openapi.yml\n  - openapi/_original/ucla-sis-courses-openapi.yml\n  - openapi/_original/ucla-sis-dictionary-openapi.yml\n  - openapi/_original/ucla-sis-production-calendar-jobs-openapi.yml\n  - openapi/_original/ucla-sis-verify-connectivity-openapi.yml\n  - openapi/_original/ucla-myucla-menu-data-openapi.yml\n  scopes:\n  - read\n  - write\n  credential_issuance: >-\n    App Key and App Secret, issued after an access request is approved in the developer portal.\n    Developers create an App, choose one or more API Products,\
  \ and the owning campus unit\n    approves. There is no public or dynamic client registration.\n  observed_enforcement: >-\n    HTTP 401 with {\"fault\":{\"faultstring\":\"Invalid access token\",\"detail\":{\"errorcode\":\n    \"oauth.v2.InvalidAccessToken\"}}} on a documented SIS route with no token present.\n  pkce_advertised: false\n  discovery_document: none\n  notes: >-\n    The contracts declare only `read` and `write` as scopes, across all six SIS products. There\n    is no per-product or per-resource scope, so an approved credential is coarse by design and\n    the real access boundary is the API Product an app is subscribed to, not the token scope.\n- name: UCLA API Gateway API key (header)\n  type: apiKey\n  x-operator: institution\n  in: header\n  parameter: x-apikey\n  declared_in:\n  - openapi/_original/ucla-weather-openapi.yml\n  observed_enforcement: HTTP 401 on https://api.ucla.edu/weather/api with no key present.\n  notes: >-\n    The UCLA Weather contract is the only\
  \ one of the seven that uses a header API key rather\n    than OAuth 2.0, and the only one written in OpenAPI 3.0.3 rather than Swagger 2.0. Two\n    credential models on one gateway is an inconsistency worth flagging, not a defect in either.\n- name: UCLA Shibboleth identity provider (SAML 2.0 / SAML 1.1)\n  type: saml\n  x-operator: institution\n  entity_id: urn:mace:incommon:ucla.edu\n  metadata_url: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aucla.edu\n  registration_authority: https://incommon.org\n  scope: ucla.edu\n  sso_endpoints:\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n    location: https://shb.ais.ucla.edu/shibboleth-idp/profile/SAML2/POST/SSO\n  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    location: https://shb.ais.ucla.edu/shibboleth-idp/profile/SAML2/Redirect/SSO\n  - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest\n    location: https://shb.ais.ucla.edu/shibboleth-idp/profile/Shibboleth/SSO\n  attribute_authority:\n\
  \  - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n    location: https://shb.ais.ucla.edu:8443/shibboleth-idp/profile/SAML2/SOAP/AttributeQuery\n  - binding: urn:oasis:names:tc:SAML:1.0:bindings:SOAP-binding\n    location: https://shb.ais.ucla.edu:8443/shibboleth-idp/profile/SAML1/SOAP/AttributeQuery\n  entity_categories:\n  - http://id.incommon.org/category/research-and-scholarship\n  - http://refeds.org/category/research-and-scholarship\n  - http://id.incommon.org/category/registered-by-incommon\n  assurance_certification:\n  - https://refeds.org/sirtfi\n  security_contact: security@it.ucla.edu\n  notes: >-\n    This is the credential every UCLA human authentication path ultimately terminates at,\n    including sign-in to the developer portal itself (/saml_login). It is machine-readable,\n    signed, and federated into eduGAIN through InCommon — the single most under-catalogued\n    institution-operated API surface class in higher education.\n- name: BruinLearn (Canvas) OAuth 2.0\
  \ and LTI 1.3\n  type: oauth2\n  x-operator: tenant\n  observed_enforcement: >-\n    HTTP 401 {\"status\":\"unauthenticated\",\"errors\":[{\"message\":\"user authorization required\"}]}\n    on https://bruinlearn.ucla.edu/api/v1/accounts.\n  public_metadata: https://bruinlearn.ucla.edu/api/lti/security/jwks\n  notes: >-\n    UCLA's students and courses, Instructure's authorization server and contract. Recorded as\n    a relationship; no Canvas contract is saved under this institution.\nunauthenticated_surfaces:\n- url: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aucla.edu\n  x-operator: institution\n  note: Signed SAML metadata, anonymously readable.\n- url: https://developer.api.ucla.edu/sites/default/files/apidoc_specs/\n  x-operator: institution\n  note: >-\n    Seven OpenAPI documents, anonymously readable. The portal gates the interactive console\n    behind campus sign-in but does not gate the underlying specification files.\n- url: https://bruinlearn.ucla.edu/api/lti/security/jwks\n\
  \  x-operator: tenant\n  note: LTI 1.3 platform JWKS, anonymously readable.\nself_service: false\nself_service_note: >-\n  No UCLA API can be reached by an unaffiliated developer. Every credential path requires a\n  UCLA logon, and the portal states that \"Most APIs, except those available for public\n  consumption, are only visible after log on.\"\nsupport_contact: api-support@it.ucla.edu\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucla/refs/heads/main/authentication/ucla-authentication.yml
summary_line: 4 schemes
tags:
- University
- Higher Education
- Education
- United States
- California
- UC System
- Public Research University
- Course Catalog
- Student Information
- Identity Federation
- Research Repository
- Library
- IIIF
- Campus Life
---
