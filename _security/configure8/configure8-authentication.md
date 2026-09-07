---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: configure8-c8-public-api-openapi.json
  format: json
  label: Configure8 REST API
  slug: idp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-c8-public-api-openapi.json
- filename: configure8-catalog-entities-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Entities API
  slug: configure8-catalog-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-entities-api-openapi.yml
- filename: configure8-catalog-relations-api-openapi.yml
  format: yaml
  label: Configure8 Catalog Relations API
  slug: configure8-catalog-relations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-catalog-relations-api-openapi.yml
- filename: configure8-deployments-api-openapi.yml
  format: yaml
  label: Configure8 Deployments API
  slug: configure8-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-deployments-api-openapi.yml
- filename: configure8-scorecards-api-openapi.yml
  format: yaml
  label: Configure8 Scorecards API
  slug: configure8-scorecards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-scorecards-api-openapi.yml
- filename: configure8-users-api-openapi.yml
  format: yaml
  label: Configure8 Users API
  slug: configure8-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/openapi/configure8-users-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Configure8 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Configure8 secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Configure8
provider_slug: configure8
scheme_count: 2
schemes:
- description: 'The documented authentication mechanism for the Public API. "Authentication is performed via Api-Key Header. All API calls must be authenticated and made over HTTPS." The docs'' own example is `curl https://app.configure8.io/public/v1/catalog/entities --header "Api-Key: my_api_key"`.'
  in: header
  key_prefix: c8ak
  lifecycle:
    attributes:
    - name
    - expiration period
    - scope
    - role
    creation: Settings > API Key Management > Add API Key
    expiry: mandatory expiration period chosen at creation
    permission_model: '"Every user has the ability to generate an API key that matches to the permissions associated with their account." A key can never exceed its creator''s permissions, and RBAC ownership (Owner / Viewer per credential, catalog entity, scorecard and self-service action) then decides what that key may touch.'
    retrieval: Shown once at creation and irretrievable afterwards — "Configure8 API keys are irretrievable, therefore this is the only time it is shown to you"
    revocation: Admins can see and revoke every key in the organization; users can manage only keys they created. Expired keys remain listed alongside active ones.
    roles:
    - name: Admin
      note: only admins can create keys with the Admin role
    - name: User
    scopes:
    - default: true
      name: read
    - default: false
      name: write
      note: both admins and regular users may add write to a key's scope
  name: api-key
  parameter: Api-Key
  plan_gating: API access is an Enterprise-plan feature. The pricing table's "API Access" row reads "No" for the Free plan.
  primary: true
  secret_scanning: Registered with GitHub secret scanning; the docs cite the prefix as the reason the format supports it
  sources:
  - openapi/configure8-c8-public-api-openapi.json
  - https://configure8.io/docs-sub/configure8-product-docs/fundamentals/settings/api-key-management
  type: apiKey
- applies_to: SCIM and Private SCIM operations
  bearerFormat: JWT
  description: Declared in the contract and attached as the only security requirement on the 19 SCIM operations (/public/v2/scim/* and the Private SCIM config at /api/v1/scim). The documentation does not describe how this token is obtained; SCIM provisioning is set up through the identity-management settings for Okta or Microsoft Entra ID rather than by a developer minting a token.
  name: bearer
  primary: false
  scheme: bearer
  sources:
  - openapi/configure8-c8-public-api-openapi.json
  type: http
slug: configure8-authentication
source_filename: configure8-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://configure8.io/docs-sub/configure8-product-docs/reference/api-documentation;\n  https://configure8.io/docs-sub/configure8-product-docs/fundamentals/settings/api-key-management;\n  https://configure8.io/docs-sub/configure8-product-docs/fundamentals/role-based-access-control;\n  openapi/configure8-c8-public-api-openapi.json\ndocs: https://configure8.io/docs-sub/configure8-product-docs/reference/api-documentation\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  primary: static API key in the Api-Key header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  transport: HTTPS required for every call\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  primary: true\n  key_prefix: c8ak\n  secret_scanning: >-\n    Registered with GitHub secret scanning; the docs cite the prefix as the reason the\n    format supports it\n  description: >-\n    The documented\
  \ authentication mechanism for the Public API. \"Authentication is performed\n    via Api-Key Header. All API calls must be authenticated and made over HTTPS.\" The docs'\n    own example is\n    `curl https://app.configure8.io/public/v1/catalog/entities --header \"Api-Key: my_api_key\"`.\n  lifecycle:\n    creation: Settings > API Key Management > Add API Key\n    attributes:\n    - name\n    - expiration period\n    - scope\n    - role\n    scopes:\n    - name: read\n      default: true\n    - name: write\n      default: false\n      note: both admins and regular users may add write to a key's scope\n    roles:\n    - name: Admin\n      note: only admins can create keys with the Admin role\n    - name: User\n    permission_model: >-\n      \"Every user has the ability to generate an API key that matches to the permissions\n      associated with their account.\" A key can never exceed its creator's permissions, and\n      RBAC ownership (Owner / Viewer per credential, catalog entity,\
  \ scorecard and\n      self-service action) then decides what that key may touch.\n    retrieval: >-\n      Shown once at creation and irretrievable afterwards — \"Configure8 API keys are\n      irretrievable, therefore this is the only time it is shown to you\"\n    revocation: >-\n      Admins can see and revoke every key in the organization; users can manage only keys\n      they created. Expired keys remain listed alongside active ones.\n    expiry: mandatory expiration period chosen at creation\n  plan_gating: >-\n    API access is an Enterprise-plan feature. The pricing table's \"API Access\" row reads\n    \"No\" for the Free plan.\n  sources:\n  - openapi/configure8-c8-public-api-openapi.json\n  - https://configure8.io/docs-sub/configure8-product-docs/fundamentals/settings/api-key-management\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  primary: false\n  description: >-\n    Declared in the contract and attached as the only security requirement on the\
  \ 19 SCIM\n    operations (/public/v2/scim/* and the Private SCIM config at /api/v1/scim). The\n    documentation does not describe how this token is obtained; SCIM provisioning is set up\n    through the identity-management settings for Okta or Microsoft Entra ID rather than by\n    a developer minting a token.\n  applies_to: SCIM and Private SCIM operations\n  sources:\n  - openapi/configure8-c8-public-api-openapi.json\nsuperseded_schemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  status: superseded\n  reason: >-\n    This scheme comes only from openapi/_original/configure8-openapi.yml and the five split\n    files derived from it, which are a best-effort reconstruction written from the docs, not\n    a harvested contract — that file says so in its own info.description. The provider's\n    published contract and its documentation both use the `Api-Key` header, not\n    `Authorization`. Recorded here so a later derive pass does not resurrect it.\n  sources:\n\
  \  - openapi/configure8-catalog-entities-api-openapi.yml\n  - openapi/configure8-catalog-relations-api-openapi.yml\n  - openapi/configure8-deployments-api-openapi.yml\n  - openapi/configure8-scorecards-api-openapi.yml\n  - openapi/configure8-users-api-openapi.yml\ndocument_level_security:\n  declared: false\n  note: >-\n    The published spec sets no top-level `security`, leaving 52 of 71 operations with no\n    stated requirement even though the docs say every call must be authenticated. The gap is\n    corrected in overlays/configure8-c8-public-api-overlay.yaml rather than by editing the\n    harvested document.\nportal_sso:\n  note: >-\n    Distinct from API authentication. Portal sign-in supports SSO (Okta, Microsoft Entra ID),\n    Sign in with Google and email; SSO is an Enterprise feature. SCIM handles user and group\n    provisioning.\n  docs: https://configure8.io/docs-sub/configure8-product-docs/fundamentals/settings/identity-management\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/configure8/refs/heads/main/authentication/configure8-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Catalog
- Cloud Cost
- Developer Experience
- DevOps
- Internal Developer Portal
- Platform Engineering
- Scorecards
- Self-Service
- Service Catalog
- SRE
---
