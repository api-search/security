---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Stensul Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stensul declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Stensul
provider_slug: stensul
scheme_count: 0
schemes: []
slug: stensul-authentication
source_filename: stensul-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://stensul.com/integrations/stensul-content-api/,\n  https://stensul.com/integrations/stensul-user-api/,\n  https://stensul.com/security-trust-center/\nname: Stensul Authentication\nderivable_from_spec: false\nderivable_note: >-\n  No OpenAPI or other machine-readable contract is published, so securitySchemes\n  could not be derived. Everything below is read from Stensul's own public\n  integration and security pages, which describe the auth model in prose without\n  naming a token endpoint, grant type, scope, or base URL.\napi_authentication:\n- api: Stensul Content API\n  scheme_type: oauth2\n  flow: client_credentials\n  flow_confidence: medium\n  flow_evidence: >-\n    Stensul describes it as \"OAuth server-to-server authentication\", which is\n    the client-credentials grant in all but name. The exact grant string, token\n    endpoint and token lifetime are not published.\n  token_endpoint: null\n  scopes_published:\
  \ false\n  additional_controls:\n  - control: ip-allowlist\n    detail: >-\n      \"IP address allowlists\" — callers must originate from addresses registered\n      with Stensul. This is a hard gate on programmatic access: an agent or CI\n      job on an unregistered egress IP cannot call the API even with a valid\n      token.\n  source: https://stensul.com/integrations/stensul-content-api/\n- api: Stensul User API\n  scheme_type: oauth2\n  flow: client_credentials\n  flow_confidence: medium\n  flow_evidence: >-\n    Same \"OAuth server-to-server authentication\" language as the Content API.\n  token_endpoint: null\n  scopes_published: false\n  additional_controls:\n  - control: ip-allowlist\n    detail: IP address allowlists, as with the Content API.\n  - control: scim\n    detail: >-\n      Stensul states the User API \"supports SCIM provisioning standards\". The\n      SCIM version (2.0 vs 1.1), the schema URNs, and the\n      /ServiceProviderConfig endpoint are not published, and\
  \ a probe of\n      app.stensul.com/scim/v2/ServiceProviderConfig returns the application's\n      SPA HTML shell rather than a SCIM document. Recorded as a vendor\n      assertion, not a verified conformance.\n  source: https://stensul.com/integrations/stensul-user-api/\nend_user_authentication:\n  note: >-\n    Distinct from API auth. Stensul's application supports enterprise SSO via\n    OAuth 2.0 / OpenID Connect and SAML 2.0, with published integration pages for\n    Okta, Microsoft Entra ID (Azure AD), Ping Identity, Duo and Google Workspace.\n    This is human sign-in to the product, not machine access to the APIs.\n  protocols:\n  - OAuth 2.0\n  - OpenID Connect\n  - SAML 2.0\n  identity_providers:\n  - name: Okta\n    url: https://stensul.com/integrations/stensul-okta-integration/\n  - name: Microsoft Entra ID / Azure AD\n    url: https://stensul.com/integrations/stensul-azure-ad-integration/\n  - name: Ping Identity\n    url: https://stensul.com/integrations/stensul-ping-identity-integration/\n\
  \  - name: Duo\n    url: https://stensul.com/integrations/stensul-duo-integration/\n  - name: Google Workspace\n    url: https://stensul.com/integrations/google-workplace-integration/\n  - name: SAML 2.0 (generic)\n    url: https://stensul.com/integrations/stensul-saml-integration/\n  source: https://stensul.com/security-trust-center/\ngaps:\n- No token endpoint URL published.\n- No grant type named explicitly.\n- No scope or permission reference published — scopes/ is therefore not written.\n- No credential-provisioning self-service; keys are issued through the account team.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stensul/refs/heads/main/authentication/stensul-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Email
- Email Marketing
- Marketing
- Marketing Automation
- Content Management
- Landing Pages
- Marketing Operations
- Enterprise Software
- Governance
- Collaboration
- Software-as-a-Service
---
