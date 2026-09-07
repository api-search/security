---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Voltaiq Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voltaiq declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Voltaiq
provider_slug: voltaiq
scheme_count: 0
schemes: []
slug: voltaiq-authentication
source_filename: voltaiq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://www.voltaiq.com/security\ndocs:\n- https://www.voltaiq.com/security\nnote: >-\n  Nothing here is derived from a specification - Voltaiq publishes no OpenAPI, so\n  derive-authentication.py produced no profile (0 auth profiles, 0 errors). Everything below is\n  read from Voltaiq's own public security page. The API authentication model itself is NOT\n  public: Voltaiq states it ships \"an API that enables flexible custom integrations\" but the\n  same page says \"Full technical documentation is available upon request\", so the scheme an API\n  client would present (key, bearer, session, mTLS) is unknown and is recorded as unknown\n  rather than guessed.\nplatform_authentication:\n  sso: true\n  protocol: SAML 2.0\n  identity_providers:\n  - Okta\n  - Azure AD\n  - Microsoft 365\n  - other standard identity providers\n  mfa: null\n  rbac: true\n  evidence: >-\n    \"Our platform supports SSO and identity federation via\
  \ SAML 2.0, including Okta, Azure AD,\n    Microsoft 365, and other standard identity providers.\" / \"Voltaiq offers many security\n    features including SAML SSO, robust authentication, and role-based access controls.\"\napi_authentication:\n  documented: false\n  scheme: unknown\n  note: >-\n    No public API reference exists. The Voltaiq Analytics Studio Python client\n    (`voltaiq_studio`) runs pre-authenticated inside the customer's own hosted notebook\n    environment and takes no credential argument in any of Voltaiq's public example notebooks,\n    so no client-side auth flow is observable from the public surface.\ndata_transport:\n  ingest: SSH & SFTP (encrypted) - \"Secure data upload is handled via SSH & SFTP encryption\"\n  direction: outbound-only - \"Outbound-only data upload - no inbound connections to your\n    network are required\"\n  browser_access: HTTPS\n  tenancy: single-tenant - dedicated infrastructure and a dedicated AWS VPC per customer\nsecurity_schemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltaiq/refs/heads/main/authentication/voltaiq-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Batteries
- Energy Storage
- Manufacturing
- Analytics
- Industrial IoT
- Data Management
- Quality
- Electric Vehicles
- Enterprise Software
---
