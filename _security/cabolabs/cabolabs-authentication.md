---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Cabolabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: CaboLabs declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: CaboLabs
provider_slug: cabolabs
scheme_count: 0
schemes: []
slug: cabolabs-authentication
source_filename: cabolabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://atomik.app/documentation/security and\n  https://atomik.app/documentation/getting_started (Atomik);\n  https://github.com/ppazos/cabolabs-ehrserver/wiki/API-error-codes-and-messages and\n  the published Insomnia collection api/EHRServer_2_0_API_Insomnia.json (EHRServer).\n  Read 2026-09-02.\ndocs: https://atomik.app/documentation/security\nnote: >-\n  Derived by SEARCH of the provider's own security and getting-started\n  documentation, not from an OpenAPI - CaboLabs publishes no machine-readable\n  contract, so there is no securitySchemes block to parse.\napis:\n- api: Atomik openEHR REST API\n  schemes:\n  - id: atomik_jwt_bearer\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    in: header\n    header: Authorization\n    value_pattern: 'Authorization: Bearer {token}'\n    token_endpoint: POST /api/v1/auth\n    token_endpoint_note: >-\n      Documented two ways in CaboLabs' own docs, which disagree\
  \ on how credentials\n      are passed. The security page and the getting-started curl both show\n      Content-Type application/x-www-form-urlencoded with email and password form\n      fields; the getting-started quick-start snippet at the top of the same page\n      shows them as QUERY STRING parameters\n      (POST /api/v1/auth?email=YOUR_EMAIL&password=YOUR_PASS). Recorded as\n      published - not reconciled, because the docs do not reconcile it.\n    token_response: '{\"token\":\"eyJ...\"}'\n    expiry: 24 hours by default, configurable to match the customer security policy\n    refresh: >-\n      No refresh-token flow is documented. On expiry the client re-authenticates\n      against POST /api/v1/auth for a fresh JWT.\n    applied_to: All API endpoints other than the auth endpoint itself.\n  - id: atomik_application_token\n    type: apiKey\n    in: header\n    header: Authorization\n    description: >-\n      Application-level access tokens for integrations with no human user\
  \ - a\n      background service, a mobile app, or an integration engine. Created by an\n      Atomik administrator and configured in the external system. Atomik trusts the\n      token and DELEGATES user-level authorization to the calling application.\n      Any token is revocable instantly from the admin panel with no code change or\n      deployment.\n    revocation: instant, from the admin panel\n  - id: atomik_keycloak_oidc\n    type: openIdConnect\n    status: supported-integration\n    description: >-\n      Atomik can delegate authentication entirely to an external identity provider.\n      CaboLabs explicitly recommends Keycloak for self-hosted OAuth2/OIDC, RBAC,\n      SSO and MFA. No discovery document, issuer URL, scope list or client\n      registration procedure is published - the integration is scoped per\n      deployment, which is why scopes/ carries no artifact for this provider.\n  audit_headers:\n    note: >-\n      Atomik requires openEHR audit provenance on writes,\
  \ carried in custom request\n      headers rather than the body. These are not authentication, but a write is\n      rejected without them, so an agent must send them.\n    headers:\n    - name: openEHR-AUDIT_DETAILS.committer\n      example: 'name=\"John Doe, MD\", external_ref.id=\"BC8132EA-8F4A-11E7-BB31-BE2E44B06B35\", external_ref.namespace=\"demographic\", external_ref.type=\"PERSON\"'\n      required: true\n    - name: openEHR-AUDIT_DETAILS.description\n      example: 'value=\"Created EHR by XYZ\"'\n      required: false\n  console_auth:\n    method: username + password\n    optional_hardening:\n    - Google reCAPTCHA on the login form\n    - Two-factor authentication via TOTP mobile app\n    note: Both are described as \"available on request\", i.e. not on by default.\n  roles:\n  - role: Administrators\n    access: Full Web Console access - templates, queries, audit logs, system configuration.\n  - role: API users\n    access: REST API only, via the auth endpoint and a JWT.\n\
  - api: CaboLabs EHRServer REST API\n  schemes:\n  - id: ehrserver_login_token\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    token_endpoint: POST /rest/v1/auth\n    description: >-\n      EHRServer authenticates against a login endpoint that returns a token, in\n      JSON or XML (the published Insomnia collection carries both a \"login JSON\"\n      and a \"login XML\" request against /rest/v1/auth). Login is multi-tenant:\n      the documented 401 error codes e01.0006 through e01.0008 show that an\n      organization number is a required credential alongside username and password,\n      and that a user must be associated with the organization it names.\n    multi_tenant: true\n    organization_scoped: true\n  - id: ehrserver_sync_key\n    type: apiKey\n    description: >-\n      The synchronization endpoints under /sync are authenticated with a separate\n      scoped JWT (the published collection's development environment carries a\n      sync_key\
  \ whose payload declares \"scope\":\"sync\"). Scoped to synchronization\n      only; not a general API credential.\n    scope: sync\ngaps:\n- No OAuth2 authorization-server metadata, no /.well-known/openid-configuration, and no published scope list on any CaboLabs host - every /.well-known/ probe on cabolabs.com returned 404 and every one on atomik.app returned an SPA shell.\n- No documented API-key prefix convention, no key-rotation policy, and no documented rate or lockout behaviour on repeated auth failure for Atomik.\n- Atomik's own docs give two different credential-passing shapes for the same POST /api/v1/auth call (form-encoded body vs query string); an integrator must try both.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cabolabs/refs/heads/main/authentication/cabolabs-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Health
- Healthcare
- Interoperability
- openEHR
- FHIR
- HL7
- Clinical Data Repository
- Electronic Health Records
- Standards
- SNOMED CT
- DICOM
- Medical Records
- Uruguay
---
