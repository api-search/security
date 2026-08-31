---
api_key_in: []
api_specs:
- filename: lakekeeper-generic-table-api-openapi.yml
  format: yaml
  label: Lakekeeper Generic Table (Data) API
  slug: lakekeeper-generic-table-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-generic-table-api-openapi.yml
- filename: lakekeeper-authorization-api-openapi.yml
  format: yaml
  label: Lakekeeper Authorization API
  slug: lakekeeper-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-authorization-api-openapi.yml
- filename: lakekeeper-catalog-api-api-openapi.yml
  format: yaml
  label: Lakekeeper Catalog API
  slug: lakekeeper-catalog-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-catalog-api-api-openapi.yml
- filename: lakekeeper-configuration-api-api-openapi.yml
  format: yaml
  label: Lakekeeper Configuration API
  slug: lakekeeper-configuration-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-configuration-api-api-openapi.yml
- filename: lakekeeper-oauth2-api-api-openapi.yml
  format: yaml
  label: Lakekeeper OAuth2 API
  slug: lakekeeper-oauth2-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-oauth2-api-api-openapi.yml
- filename: lakekeeper-permissions-cedar-api-openapi.yml
  format: yaml
  label: Lakekeeper Permissions Cedar API
  slug: lakekeeper-permissions-cedar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-permissions-cedar-api-openapi.yml
- filename: lakekeeper-permissions-openfga-api-openapi.yml
  format: yaml
  label: Lakekeeper Permissions Openfga API
  slug: lakekeeper-permissions-openfga-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-permissions-openfga-api-openapi.yml
- filename: lakekeeper-project-api-openapi.yml
  format: yaml
  label: Lakekeeper Project API
  slug: lakekeeper-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-project-api-openapi.yml
- filename: lakekeeper-role-api-openapi.yml
  format: yaml
  label: Lakekeeper Role API
  slug: lakekeeper-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-role-api-openapi.yml
- filename: lakekeeper-server-api-openapi.yml
  format: yaml
  label: Lakekeeper Server API
  slug: lakekeeper-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-server-api-openapi.yml
- filename: lakekeeper-tasks-api-openapi.yml
  format: yaml
  label: Lakekeeper Tasks API
  slug: lakekeeper-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-tasks-api-openapi.yml
- filename: lakekeeper-user-api-openapi.yml
  format: yaml
  label: Lakekeeper User API
  slug: lakekeeper-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-user-api-openapi.yml
- filename: lakekeeper-warehouse-api-openapi.yml
  format: yaml
  label: Lakekeeper Warehouse API
  slug: lakekeeper-warehouse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/openapi/lakekeeper-warehouse-api-openapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Lakekeeper Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Lakekeeper secures its APIs with http, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Lakekeeper
provider_slug: lakekeeper
scheme_count: 2
schemes:
- applies_to: all three APIs (catalog, management, generic-table) and the Plus management API
  bearerFormat: JWT
  default: true
  detail: Declared as the top-level `security` requirement on the Management, Generic Table and Plus documents. The token is validated on signature (via the IdP's jwks_uri), issuer, and — when configured — audience.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lakekeeper-catalog-api-openapi.yml
  - openapi/lakekeeper-generic-table-api-openapi.yml
  - openapi/lakekeeper-management-api-openapi.yml
  - openapi/lakekeeper-management-plus-api-openapi.yml
  type: http
- applies_to: Iceberg REST Catalog API
  deprecated_note: The catalog-hosted token endpoint (operationId getToken) is marked deprecated in the upstream Apache Iceberg specification in favour of an external authorization server. The Iceberg spec's own guidance — carried in the scheme description Lakekeeper serves — is to substitute tokenUrl with the external authorization server's full token path.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /v1/oauth/tokens
  name: OAuth2
  scopes_artifact: scopes/lakekeeper-scopes.yml
  sources:
  - openapi/lakekeeper-catalog-api-openapi.yml
  type: oauth2
slug: lakekeeper-authentication
source_filename: lakekeeper-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  https://docs.lakekeeper.io/docs/latest/authentication/, https://docs.lakekeeper.io/docs/latest/configuration/,\n  https://docs.lakekeeper.io/docs/latest/authorization/, openapi/lakekeeper-catalog-api-openapi.yml,\n  openapi/lakekeeper-management-api-openapi.yml, openapi/lakekeeper-generic-table-api-openapi.yml,\n  openapi/lakekeeper-management-plus-api-openapi.yml\ndocs: https://docs.lakekeeper.io/docs/latest/authentication/\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - clientCredentials\n  api_keys: false\n  note: >-\n    Lakekeeper has NO API-key path. Every caller presents a bearer JWT, and Lakekeeper does not mint those — it\n    validates tokens issued by an identity provider the operator configures. That is a deliberate design choice\n    for self-hosted software: there is no vendor account system to hold keys in.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n\
  \  bearerFormat: JWT\n  applies_to: all three APIs (catalog, management, generic-table) and the Plus management API\n  default: true\n  detail: >-\n    Declared as the top-level `security` requirement on the Management, Generic Table and Plus documents. The\n    token is validated on signature (via the IdP's jwks_uri), issuer, and — when configured — audience.\n  sources:\n  - openapi/lakekeeper-catalog-api-openapi.yml\n  - openapi/lakekeeper-generic-table-api-openapi.yml\n  - openapi/lakekeeper-management-api-openapi.yml\n  - openapi/lakekeeper-management-plus-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /v1/oauth/tokens\n    scopes: 1\n  applies_to: Iceberg REST Catalog API\n  deprecated_note: >-\n    The catalog-hosted token endpoint (operationId getToken) is marked deprecated in the upstream Apache Iceberg\n    specification in favour of an external authorization server. The Iceberg spec's own guidance — carried in the\n    scheme\
  \ description Lakekeeper serves — is to substitute tokenUrl with the external authorization server's full\n    token path.\n  sources:\n  - openapi/lakekeeper-catalog-api-openapi.yml\n  scopes_artifact: scopes/lakekeeper-scopes.yml\nidentity_providers:\n  configuration:\n  - name: LAKEKEEPER__OPENID_PROVIDER_URI\n    detail: >-\n      Points at the operator's IdP. The provider MUST serve /.well-known/openid-configuration, and that document\n      must define jwks_uri and issuer.\n  - name: LAKEKEEPER__OPENID_PROVIDERS\n    since: v0.13.0\n    detail: >-\n      Configure several providers simultaneously — e.g. Okta for humans and a cloud OIDC issuer for service\n      accounts. Backwards-compatible with the single-provider setting.\n  - name: LAKEKEEPER__OPENID_AUDIENCE\n    detail: >-\n      Validates the token's `aud` claim. RECOMMENDED in every deployment, so a token leaked for another\n      application on the same IdP cannot be used to reach data in Lakekeeper.\n  - name: subject claim\
  \ fallback\n    detail: >-\n      The OpenID subject-claim setting accepts a comma-separated list; the first matching claim in the token wins,\n      which eases integration across heterogeneous IdPs.\n  documented_idps:\n  - Keycloak\n  - Microsoft Entra ID (Azure AD)\n  - Okta (with DPoP on the role provider, opt-out to Bearer)\n  - Any OIDC-compliant provider\n  kubernetes:\n    supported: true\n    detail: >-\n      Kubernetes service-account tokens are accepted as an alternative authenticator.\n      LAKEKEEPER__KUBERNETES_AUTHENTICATION_SUBJECT_SOURCE=username derives the Lakekeeper user id from\n      `system:serviceaccount:<namespace>:<name>` — stable across clusters — instead of the per-cluster uid\n      (the default), so roles and instance admins can be pre-provisioned.\nprincipal_identifiers:\n  oidc: 'oidc~<subject from the provider>'\n  note: Roles bound to an external source system carry provider-id + source-id rather than being managed in Lakekeeper.\nmachine_clients:\n\
  \  flow: OAuth2 client_credentials against the operator's IdP\n  detail: >-\n    All common Iceberg clients and IdPs support client_credentials. The documentation walks through app\n    registration for Keycloak and Entra ID, including the exact spark.sql.catalog.<name>.oauth2-server-uri\n    configuration engines need.\n  warning: >-\n    From the Flink guide — inject TOKEN / OAUTH_* through Flink's env.java.opts or cluster secret management;\n    never pass secrets on the `flink run` command line in production.\nauthorization:\n  note: >-\n    Authentication and authorization are separate and separately pluggable. After a token is validated, the\n    configured Authorizer decides what the principal may do: AllowAll (default, no authorization), OpenFGA\n    (Zanzibar-style ReBAC, the recommended production choice), an Open Policy Agent bridge for engine-level\n    delegation, or Cedar in Lakekeeper+.\n  admission_gates:\n    since: v0.13.0\n    detail: >-\n      A coarse allow/deny hook\
  \ that runs AFTER authentication and BEFORE any handler — distinct from the\n      per-resource Authorizer. Used to consult an external entitlement service, suspend a tenant, or honour a\n      token deny-list. Gates may also contribute resolved roles and can see the caller's bearer token. Only an\n      exact 403 is read as an authoritative deny; every other non-2xx makes the gate fail closed with a 503.\n    docs: https://docs.lakekeeper.io/docs/latest/admission/\n  actions_endpoints: >-\n    get_server_actions, get_project_actions, get_warehouse_actions, get_namespace_actions, get_table_actions,\n    get_view_actions, get_generic_table_actions, get_role_actions and get_user_actions answer \"what may this\n    principal do here?\" — the correct pre-flight for an agent, and the way to tell a permission failure apart from\n    a nonexistent object.\n  docs: https://docs.lakekeeper.io/docs/latest/authorization/\ngaps:\n- No API keys, no personal access tokens — an operator must stand up\
  \ an IdP before Lakekeeper is usable in production.\n- >-\n  The catalog document's OAuth2 tokenUrl is a relative path (/v1/oauth/tokens) pointing at a deprecated endpoint;\n  a client must be told the external authorization server out of band.\n- The Management API declares no scopes; authorization is entirely delegated to the Authorizer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakekeeper/refs/heads/main/authentication/lakekeeper-authentication.yml
summary_line: http/oauth2/openIdConnect · 2 schemes
tags:
- apache-iceberg
- data-catalog
- lakehouse
- Open-Source
- rust
- data-governance
- access-control
- object-storage
- Metadata
- self-hosted
- openfga
- data-engineering
---
