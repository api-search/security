---
api_key_in:
- header
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Guidewheel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Guidewheel secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Guidewheel
provider_slug: guidewheel
scheme_count: 2
schemes:
- example: 'curl "https://<base-url>/api/v1/devices" -H "x-api-key: $API_KEY"'
  in: header
  name: ApiKeyHeader
  parameter_name: x-api-key
  scope: Company-scoped. Each API key only has access to the company data associated with it.
  sources:
  - https://support.guidewheel.app/en/articles/15696169-guidewheel-api-cmms-erp-integration-guide
  status: current
  transport: HTTPS required for all requests.
  type: apiKey
- in: query
  name: ApiKeyQuery
  note: Older integrations may use an api_key query parameter; the provider documents this as deprecated in favour of the x-api-key header.
  parameter_name: api_key
  sources:
  - https://support.guidewheel.app/en/articles/15696169-guidewheel-api-cmms-erp-integration-guide
  status: deprecated
  type: apiKey
slug: guidewheel-authentication
source_filename: guidewheel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://support.guidewheel.app/en/articles/15696169-guidewheel-api-cmms-erp-integration-guide\ndocs: https://support.guidewheel.app/en/articles/15696169-guidewheel-api-cmms-erp-integration-guide\nnote: >-\n  Derived from the provider's published API and account documentation, not from an\n  OpenAPI document — Guidewheel does not publish a machine-readable contract (the\n  detailed technical API guide is password protected and provided on request).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  sso: true\n  mfa: true\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  status: current\n  scope: >-\n    Company-scoped. Each API key only has access to the company data associated with\n    it.\n  transport: HTTPS required for all requests.\n  example: 'curl \"https://<base-url>/api/v1/devices\" -H \"x-api-key: $API_KEY\"'\n  sources:\n  - https://support.guidewheel.app/en/articles/15696169-guidewheel-api-cmms-erp-integration-guide\n\
  - name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter_name: api_key\n  status: deprecated\n  note: >-\n    Older integrations may use an api_key query parameter; the provider documents this\n    as deprecated in favour of the x-api-key header.\n  sources:\n  - https://support.guidewheel.app/en/articles/15696169-guidewheel-api-cmms-erp-integration-guide\nend_user_authentication:\n  note: >-\n    The API itself uses a company-scoped API key. The following applies to human sign-in\n    to the Guidewheel web/mobile application, not to API clients.\n  login:\n    url: https://app.guidewheel.app/\n    identifier: username (explicitly not the email address)\n    password_policy: 12-character password\n    docs: https://support.guidewheel.app/en/articles/12168446-how-to-login-to-guidewheel\n  sso:\n    supported: true\n    provider: WorkOS\n    protocols:\n    - SAML\n    - OIDC\n    identity_providers:\n    - Okta\n    - Microsoft Entra ID / Azure AD\n    - Google\n    - OneLogin\n  \
  \  - any IdP supporting SAML or OIDC\n    saml_requirements:\n      provided_by_workos:\n      - ACS URL (Assertion Consumer Service URL)\n      - SP Entity ID\n      provided_by_customer:\n      - Metadata URL (recommended)\n      - XML metadata file upload\n      - 'Manual entry: IdP Single Sign-On URL, IdP Entity ID / Issuer, X.509 signing\n        certificate'\n      attribute_mappings:\n      - email -> user.email\n      - firstName -> user.firstName\n      - lastName -> user.lastName\n    oidc_requirements:\n    - Client ID\n    - Client Secret\n    - Discovery Endpoint (.well-known/openid-configuration URL)\n    user_provisioning: false\n    mfa_on_sso: false\n    password_login_can_be_blocked: true\n    onboarding: Contact your account executive or customer success manager for an invite link.\n    docs: https://support.guidewheel.app/en/articles/14175623-how-to-set-up-single-sign-on-sso-with-guidewheel\n  mfa:\n    supported: true\n    self_service: true\n    methods:\n    - SMS\n\
  \    - WhatsApp\n    docs: https://support.guidewheel.app/en/articles/8891042-setting-up-two-factor-authentication\n  roles_and_permissions:\n    docs: https://support.guidewheel.app/en/articles/7258359-roles-and-permissions\nx-evidence:\n  fetched: '2026-08-01'\n  urls:\n  - url: https://support.guidewheel.app/en/articles/15696169-guidewheel-api-cmms-erp-integration-guide\n    http_status: 200\n  - url: https://support.guidewheel.app/en/articles/14175623-how-to-set-up-single-sign-on-sso-with-guidewheel\n    http_status: 200\n  - url: https://support.guidewheel.app/en/articles/8891042-setting-up-two-factor-authentication\n    http_status: 200\n  negative:\n  - url: https://api.guidewheel.app/.well-known/openid-configuration\n    http_status: 200\n    result: SPA HTML shell, not an OIDC discovery document\n  - url: https://api.guidewheel.app/.well-known/oauth-authorization-server\n    http_status: 200\n    result: SPA HTML shell, not an RFC 8414 document\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guidewheel/refs/heads/main/authentication/guidewheel-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Manufacturing
- Industrial IoT
- Machine Monitoring
- OEE
- FactoryOps
- Predictive Maintenance
- Energy
- Sensors
- Telemetry
---
