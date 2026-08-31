---
api_key_in: []
auth_types:
- apiKey
description: 'Sedai''s platform API is authenticated with a long-lived API token minted in the tenant console. There is no published OpenAPI, so this profile is read from Sedai''s own first-party SDK reference rather than derived from a securityScheme block. The token is a JWT with an exp claim — Sedai documents reading the expiry client-side by base64-decoding the payload — and it is scoped to one tenant: a key from one Sedai instance returns 401 against another.'
kind: authentication
layout: security
method: searched
name: Sedai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sedai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sedai
provider_slug: sedai
scheme_count: 1
schemes:
- description: Bearer API token passed by the SDK on every request to the tenant's https://{tenant}.sedai.app host. Sedai does not publish the raw header name in its public docs; the SDK sets it internally via configure({ baseUrl, apiToken }).
  expires: true
  expiry_discovery: The token is a JWT; Sedai documents decoding the payload segment to read the "exp" claim without calling the API (echo "$SEDAI_API_TOKEN" | cut -d. -f2 | base64 -d | grep exp).
  format: JWT
  in: header
  issued_at: Settings -> API Keys -> Create New Key, inside the tenant console
  name: sedaiApiToken
  sdk_env_vars:
  - SEDAI_BASE_URL
  - SEDAI_API_TOKEN
  shown_once: true
  source: REFERENCE-typescript.md#authentication
  tenant_scoped: true
  type: apiKey
slug: sedai-authentication
source_filename: sedai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://github.com/SedaiEngineering/sedai-sdk-releases/blob/main/REFERENCE-typescript.md\n  (Authentication section, API key roles, and the 401/403 troubleshooting\n  table), https://github.com/SedaiEngineering/sedai-sdk-releases/blob/main/README.md,\n  and https://docs.sedai.io/get-started/onboarding/readme/safety-and-security\n  (SAML / MFA / key management) plus\n  https://docs.sedai.io/get-started/platform/single-sign-on-rbac (OIDC + SAML SSO).\ndescription: >-\n  Sedai's platform API is authenticated with a long-lived API token minted in\n  the tenant console. There is no published OpenAPI, so this profile is read\n  from Sedai's own first-party SDK reference rather than derived from a\n  securityScheme block. The token is a JWT with an exp claim — Sedai documents\n  reading the expiry client-side by base64-decoding the payload — and it is\n  scoped to one tenant: a key from one Sedai instance returns 401 against\n\
  \  another.\nbase_url_template: https://{tenant}.sedai.app\nsummary:\n  types:\n    - apiKey\n  api_token: true\n  oauth2: false\n  openid_connect: consumer-side only (console SSO, not API auth)\n  mutual_tls: false\nschemes:\n  - name: sedaiApiToken\n    type: apiKey\n    in: header\n    format: JWT\n    issued_at: Settings -> API Keys -> Create New Key, inside the tenant console\n    shown_once: true\n    expires: true\n    expiry_discovery: >-\n      The token is a JWT; Sedai documents decoding the payload segment to read\n      the \"exp\" claim without calling the API\n      (echo \"$SEDAI_API_TOKEN\" | cut -d. -f2 | base64 -d | grep exp).\n    tenant_scoped: true\n    sdk_env_vars:\n      - SEDAI_BASE_URL\n      - SEDAI_API_TOKEN\n    description: >-\n      Bearer API token passed by the SDK on every request to the tenant's\n      https://{tenant}.sedai.app host. Sedai does not publish the raw header\n      name in its public docs; the SDK sets it internally via configure({\n   \
  \   baseUrl, apiToken }).\n    source: REFERENCE-typescript.md#authentication\nroles:\n  - name: user\n    grants: All read operations — accounts, resources, recommendations, opportunities.\n  - name: admin\n    grants: >-\n      Required for every write/update operation (updateResourceSettings,\n      updateGroupSettings, updateAccountSettings). A write call made with a\n      user-role key returns 403.\nfeature_flags:\n  - name: BULK_OPPORTUNITIES_API_ENABLED\n    description: >-\n      Off by default for all tenants. getOpportunitiesForResources returns 403\n      until Sedai support enables it. A per-tenant entitlement flag, not a\n      scope — it is not discoverable from the token.\nconsole_sso:\n  protocols:\n    - SAML 2.0\n    - OIDC\n  mfa: >-\n    Sedai offers AWS SSO password policies and MFA for SaaS customers; MFA is\n    mandatory on all internal systems handling customer data.\n  rbac: true\n  docs: https://docs.sedai.io/get-started/platform/single-sign-on-rbac\n  note:\
  \ >-\n    SAML/OIDC govern human login to the Sedai console. They are NOT an\n    authorization mechanism for the platform API, which uses the console-minted\n    API token only. Sedai publishes no OAuth 2.0 authorization server and no\n    /.well-known/openid-configuration of its own.\nfailure_modes:\n  - status: 401\n    meaning: Token missing, wrong, expired, or belonging to a different tenant.\n    remediation: Re-generate the key in Settings -> API Keys; check the JWT exp claim.\n  - status: 403\n    meaning: Valid token, insufficient role, or a tenant feature flag is off.\n    remediation: Use an admin-role key for writes; contact Sedai support for the feature flag.\ngaps:\n  - No published API key prefix or header name in the public documentation.\n  - No documented key rotation policy, key expiry period, or revocation endpoint.\n  - No OAuth 2.0 / OIDC option for machine access; no scopes, so least-privilege is limited to the two coarse roles.\nmaintainers:\n  - FN: Kin Lane\n\
  \    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sedai/refs/heads/main/authentication/sedai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Optimization
- FinOps
- Kubernetes
- Cloud Cost Management
- Autonomous Operations
- Observability
- Artificial Intelligence
- DevOps
---
