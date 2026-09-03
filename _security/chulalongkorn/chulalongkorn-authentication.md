---
api_key_in: []
api_specs:
- filename: chulalongkorn-sso-openapi.yml
  format: yaml
  label: Chula SSO Authentication API
  slug: sso
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chulalongkorn/refs/heads/main/openapi/chulalongkorn-sso-openapi.yml
- filename: chulalongkorn-course-schedule-openapi.yml
  format: yaml
  label: CU-REG Course Schedule API
  slug: course-schedule
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chulalongkorn/refs/heads/main/openapi/chulalongkorn-course-schedule-openapi.yml
auth_types: []
description: 'Chulalongkorn University runs two distinct authentication stories and they do not meet. Its own campus SSO is a bespoke CAS 1.0 variant with an added application-authentication step, in production since January 2017 and documented in prose on a public wiki. Its cloud identity is a Microsoft Entra ID tenant covering both chula.ac.th and student.chula.ac.th, whose OIDC and SAML metadata are fully machine-readable. Neither is presented to developers as an API program: there is no self-service registration, no published client-credentials flow, and no developer portal at which either could be claimed.'
kind: authentication
layout: security
method: derived
name: Chulalongkorn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chulalongkorn University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Chulalongkorn University
provider_slug: chulalongkorn
scheme_count: 0
schemes: []
slug: chulalongkorn-authentication
source_filename: chulalongkorn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Evangelist Authentication\nspecificationVersion: '0.1'\nprovider: Chulalongkorn University\nproviderId: chulalongkorn\ngenerated: '2026-09-01'\nmethod: derived\nsource: >-\n  https://account.it.chula.ac.th/wiki/doku.php?id=how_does_it_work (HTTP 200) for the Chula\n  SSO servlet contract; live unauthenticated fetches of\n  https://cas.reg.chula.ac.th/class/api/course-studies and /version (both HTTP 200) for the\n  registrar API; and\n  https://login.microsoftonline.com/chula.ac.th/v2.0/.well-known/openid-configuration\n  (HTTP 200) for the institution's Entra ID tenant.\ndescription: >-\n  Chulalongkorn University runs two distinct authentication stories and they do not meet.\n  Its own campus SSO is a bespoke CAS 1.0 variant with an added application-authentication\n  step, in production since January 2017 and documented in prose on a public wiki. Its\n  cloud identity is a Microsoft Entra ID tenant covering both chula.ac.th and\n  student.chula.ac.th, whose\
  \ OIDC and SAML metadata are fully machine-readable. Neither is\n  presented to developers as an API program: there is no self-service registration, no\n  published client-credentials flow, and no developer portal at which either could be\n  claimed.\n\nmethods:\n- id: chula-sso-application-keys\n  name: Chula SSO application keys (DeeAppId / DeeAppSecret)\n  x-operator: institution\n  type: api_key\n  location: header\n  parameters:\n  - name: DeeAppId\n    description: Application identifier issued by the university.\n  - name: DeeAppSecret\n    description: Application secret issued by the university.\n  - name: DeeTicket\n    description: Service ticket obtained from the /login redirect, presented for validation.\n  protocol: Modified CAS 1.0, with application authentication added on top of ticket validation\n  onboarding: manual\n  self_service: false\n  onboarding_detail: >-\n    Keys are requested by email from the SSO's architect in the Department of Computer\n    Engineering;\
  \ the wiki names the address. There is no registration form, no console, and\n    no published turnaround or terms. This is the single largest ergonomics gap in the\n    profile: the contract is well documented and the door to it is a person's inbox.\n  documentation: https://account.it.chula.ac.th/wiki/doku.php?id=how_does_it_work\n  backend: University LDAP directory operated by the Office of Information Technology\n  status_probed: '2026-09-01'\n  status: 200\n\n- id: cu-reg-course-schedule-anonymous\n  name: CU-REG Course Schedule — no authentication\n  x-operator: institution\n  type: none\n  self_service: true\n  detail: >-\n    GET https://cas.reg.chula.ac.th/class/api/course-studies and /version both return HTTP\n    200 JSON to an unauthenticated, unkeyed request from outside the campus network. No\n    API key, no token, no CORS preflight and no rate-limit headers were observed. The\n    thirteen further endpoints the client bundle declares return HTTP 404 to the same\n    unauthenticated\
  \ caller.\n  status_probed: '2026-09-01'\n  status: 200\n\n- id: entra-id-tenant\n  name: Microsoft Entra ID tenant (OpenID Connect / SAML 2.0)\n  x-operator: federation\n  type: oidc\n  issuer: https://login.microsoftonline.com/271d5e7b-1350-4b96-ab84-52dbda4cf40c/v2.0\n  tenant_id: 271d5e7b-1350-4b96-ab84-52dbda4cf40c\n  discovery: https://login.microsoftonline.com/chula.ac.th/v2.0/.well-known/openid-configuration\n  saml_metadata: https://login.microsoftonline.com/271d5e7b-1350-4b96-ab84-52dbda4cf40c/federationmetadata/2007-06/federationmetadata.xml\n  saml_entity_id: https://sts.windows.net/271d5e7b-1350-4b96-ab84-52dbda4cf40c/\n  domains:\n  - chula.ac.th\n  - student.chula.ac.th\n  namespace_type: Managed\n  detail: >-\n    A managed (not federated) Entra tenant branded \"Chulalongkorn University\". Both the\n    OIDC discovery document and the SAML 2.0 federation metadata resolve HTTP 200 without\n    credentials. This is the institution's own identity surface running on Microsoft's\n\
  \    infrastructure, and it is the most complete machine-readable identity contract the\n    university has — but it is a tenant deployment, not an authorization server the\n    university offers to third-party developers.\n  status_probed: '2026-09-01'\n  status: 200\n\ngaps:\n- No OAuth 2.0 or OpenID Connect authorization server is offered to third-party developers\n  under any chula.ac.th host.\n- No self-service developer registration anywhere in the estate.\n- No published rate limits, quotas or terms of use for either institution-operated API.\n- CU Data Gateway, the university's central data exchange, is restricted to assigned\n  university personnel; its documentation host sits behind an Imperva bot challenge and its\n  portal (datagateway.chula.ac.th) does not answer from outside the campus network.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chulalongkorn/refs/heads/main/authentication/chulalongkorn-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Research
- Thailand
- Bangkok
- Identity Federation
- Single Sign-On
- Course Catalog
- Research Repository
- Library
- Open Access
- OAI-PMH
---
