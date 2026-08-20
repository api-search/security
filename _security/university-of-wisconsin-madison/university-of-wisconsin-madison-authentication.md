---
api_key_in: []
api_specs:
- filename: university-of-wisconsin-madison-person-api-openapi.yml
  format: yaml
  label: Person API
  slug: person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-person-api-openapi.yml
- filename: university-of-wisconsin-madison-mock-person-api-openapi.yml
  format: yaml
  label: Mock Person API
  slug: mock-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-mock-person-api-openapi.yml
- filename: university-of-wisconsin-madison-mock-person-api-certificates-openapi.yml
  format: yaml
  label: Mock Person API (Certificates)
  slug: mock-person-api-certificates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-mock-person-api-certificates-openapi.yml
- filename: university-of-wisconsin-madison-hr-api-openapi.yml
  format: yaml
  label: HR API
  slug: hr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-hr-api-openapi.yml
- filename: university-of-wisconsin-madison-mock-hr-api-openapi.yml
  format: yaml
  label: Mock HR API
  slug: mock-hr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-mock-hr-api-openapi.yml
- filename: university-of-wisconsin-madison-manifest-api-openapi.yml
  format: yaml
  label: Manifest API
  slug: manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-manifest-api-openapi.yml
- filename: university-of-wisconsin-madison-mock-manifest-api-openapi.yml
  format: yaml
  label: Mock Manifest API
  slug: mock-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-mock-manifest-api-openapi.yml
- filename: university-of-wisconsin-madison-finance-api-openapi.yml
  format: yaml
  label: Finance API
  slug: finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-finance-api-openapi.yml
- filename: university-of-wisconsin-madison-locations-api-openapi.yml
  format: yaml
  label: Locations API
  slug: locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-locations-api-openapi.yml
- filename: university-of-wisconsin-madison-enterprise-billing-api-openapi.yml
  format: yaml
  label: Enterprise Billing API
  slug: enterprise-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-enterprise-billing-api-openapi.yml
- filename: university-of-wisconsin-madison-oauth-api-openapi.yml
  format: yaml
  label: OAuth API
  slug: oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-oauth-api-openapi.yml
- filename: university-of-wisconsin-madison-course-search-api-openapi.yml
  format: yaml
  label: Public Course Search API
  slug: course-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/openapi/university-of-wisconsin-madison-course-search-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: University Of Wisconsin Madison Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: University of Wisconsin-Madison secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: University of Wisconsin-Madison
provider_slug: university-of-wisconsin-madison
scheme_count: 3
schemes:
- declared_scopes: []
  flow: clientCredentials
  name: OAuth2ClientCredentials
  purpose: Bearer access token for every gated UW-Madison enterprise API.
  token_url: https://api.wisc.edu/oauth/token
  type: oauth2
  used_by: 10 of 12 contracts — Person, Mock Person, Mock Person Certificates, HR, Mock HR, Manifest, Mock Manifest, Finance, Locations, and (by documentation, not by scheme) Enterprise Billing.
- name: basicAuth
  purpose: Presents the client_id/client_secret pair to POST https://api.wisc.edu/oauth/token in exchange for an access token. The OAuth contract notes that enabling the OAuth API product is not itself necessary in order to obtain tokens.
  scheme: basic
  type: http
  used_by: openapi/university-of-wisconsin-madison-oauth-api-openapi.yml
- name: none
  type: none
  used_by: openapi/university-of-wisconsin-madison-course-search-api-openapi.yml (public.enroll.wisc.edu) — fully open, no credential of any kind. Verified by an unauthenticated POST returning 226 and 932 course records.
slug: university-of-wisconsin-madison-authentication
source_filename: university-of-wisconsin-madison-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: derived\nsource: openapi/university-of-wisconsin-madison-oauth-api-openapi.yml\ndocs: https://git.doit.wisc.edu/interop/external-docs/api-publisher-documentation\nx-operator: institution\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  note: >-\n    UW-Madison runs two entirely separate authentication planes and conflating them is the\n    easiest mistake to make here. The API plane (api.wisc.edu, Google Apigee, org\n    doit-ipt-apigee-prod-ce29) is OAuth 2.0 client-credentials only — machine-to-machine, no\n    user context, no OIDC discovery. The human plane (login.wisc.edu) is a UW-operated\n    Shibboleth IdP speaking SAML 2.0 and OIDC for campus SSO. No published API contract\n    references the login.wisc.edu issuer.\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.wisc.edu/oauth/token\n  declared_scopes: []\n  used_by: >-\n    10 of 12\
  \ contracts — Person, Mock Person, Mock Person Certificates, HR, Mock HR, Manifest,\n    Mock Manifest, Finance, Locations, and (by documentation, not by scheme) Enterprise Billing.\n  purpose: Bearer access token for every gated UW-Madison enterprise API.\n- name: basicAuth\n  type: http\n  scheme: basic\n  used_by: openapi/university-of-wisconsin-madison-oauth-api-openapi.yml\n  purpose: >-\n    Presents the client_id/client_secret pair to POST https://api.wisc.edu/oauth/token in\n    exchange for an access token. The OAuth contract notes that enabling the OAuth API product\n    is not itself necessary in order to obtain tokens.\n- name: none\n  type: none\n  used_by: >-\n    openapi/university-of-wisconsin-madison-course-search-api-openapi.yml\n    (public.enroll.wisc.edu) — fully open, no credential of any kind. Verified by an\n    unauthenticated POST returning 226 and 932 course records.\nonboarding:\n  self_service: false\n  detail: >-\n    Access to production APIs is granted,\
  \ not signed up for. The Person API access page\n    documents an institutional access request, and every API product in the portal catalog\n    carries approvalType \"manual\". A UW NetID is required to sign in to the developer portal at\n    all, so the credential path is closed to anyone outside the institution.\n  gated_by: institutional access request + manual approval per API product\n  request_url: https://developer.wisc.edu/person-api/getting-access\n  contact: api@doit.wisc.edu\nmocks:\n  detail: >-\n    UW-Madison publishes openly readable MOCK variants on mock.api.wisc.edu for four of its\n    gated APIs (Person, Person Certificates, HR, Manifest). This is a deliberate and unusually\n    good practice for a university: the contract and the shape of the data are public even\n    though the production data is not.\n  hosts: [https://mock.api.wisc.edu]\nidentity_federation:\n  operator: institution\n  entity_id: https://login.wisc.edu/idp/shibboleth\n  saml_metadata: https://login.wisc.edu/idp/shibboleth\n\
  \  oidc_discovery: https://login.wisc.edu/.well-known/openid-configuration\n  scope: wisc.edu\n  detail: >-\n    Institution-operated Shibboleth IdP serving both SAML 2.0 and OpenID Connect. Governs campus\n    SSO and the vendor tenants (Canvas), not the API gateway.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-wisconsin-madison/refs/heads/main/authentication/university-of-wisconsin-madison-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- University
- Higher Education
- Education
- Public Research University
- United States
- Wisconsin
- Big Ten
- Association of American Universities
- Identity
- Identity Federation
- Course Catalog
- Research Repository
- Student Information System
- Human Resources
- Finance
- Curriculum
---
