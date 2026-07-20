---
api_key_in: []
auth_types:
- saml
description: ''
kind: authentication
layout: security
method: searched
name: Lanes And Planes Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lanes & Planes secures its APIs with saml across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lanes & Planes
provider_slug: lanes-and-planes
scheme_count: 1
schemes:
- application: https://app.lanes-planes.com/
  audience: end-user / workforce authentication to the Lanes & Planes application
  evidence: '"Authentication: Enterprise-wide security via Single Sign-On (SSO) supporting SAML 2.0."'
  name: SAML 2.0 Single Sign-On
  protocol: SAML 2.0
  sources:
  - https://www.lanes-planes.com/llms.txt
  type: saml
slug: lanes-and-planes-authentication
source_filename: lanes-and-planes-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.lanes-planes.com/llms.txt\ndocs: https://support.lanes-planes.com/hc/en-us\nsummary:\n  types:\n  - saml\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Derived-from-OpenAPI is not possible for this provider: Lanes & Planes publishes no\n    OpenAPI, Swagger, or other machine-readable API definition, so there are no\n    securitySchemes to aggregate. This profile is assembled from the company's own\n    published statements only.\nschemes:\n- name: SAML 2.0 Single Sign-On\n  type: saml\n  protocol: SAML 2.0\n  audience: end-user / workforce authentication to the Lanes & Planes application\n  application: https://app.lanes-planes.com/\n  sources:\n  - https://www.lanes-planes.com/llms.txt\n  evidence: >-\n    \"Authentication: Enterprise-wide security via Single Sign-On (SSO) supporting\n    SAML 2.0.\"\napi_authentication:\n  documented: false\n  status: undisclosed\n  note: >-\n    The External API (ExtAPI)\
  \ used for HRIS and identity-system synchronization is named\n    by the company but its authentication model is not published. No public developer\n    portal, API reference, credential self-service, or OpenAPI definition exists, so the\n    API-side scheme (key, bearer token, mTLS, or OAuth) is unknown. Nothing is asserted\n    here in the absence of evidence.\noauth:\n  documented: false\n  note: >-\n    No OAuth or OpenID Connect surface was found. /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server return 404 on both the marketing and\n    application hosts. No scopes/ artifact is produced, per the pipeline rule that\n    scopes/ is OAuth-only.\nidentity_integrations:\n- name: Personio\n  kind: HRIS\n  integration: native synchronization\n  marketplace: https://www.marketplace.personio.de/integrations/lanes_planes/\n- name: Workday\n  kind: HRIS\n  integration: via External API (ExtAPI)\n- name: BambooHR\n  kind: HRIS\n  integration: via External API\
  \ (ExtAPI)\n- name: HiBob\n  kind: HRIS\n  integration: via External API (ExtAPI)\nrelated:\n  conformance: conformance/lanes-and-planes-conformance.yml\n  domain_security: security/lanes-and-planes-domain-security.yml\n  trust_center: security/lanes-and-planes-trust-center.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lanes-and-planes/refs/heads/main/authentication/lanes-and-planes-authentication.yml
summary_line: saml · 1 scheme
tags:
- Company
- Travel
- Business Travel
- Travel Management
- Expense Management
- Spend Management
- Finance
- Accounting
- ERP Integration
- HRIS
- SaaS
- Germany
- Europe
---
