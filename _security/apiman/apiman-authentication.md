---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apiman-actions-api-openapi.yml
  format: yaml
  label: Apiman Actions API
  slug: apiman-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-actions-api-openapi.yml
- filename: apiman-blobs-api-openapi.yml
  format: yaml
  label: Apiman Blobs API
  slug: apiman-blobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-blobs-api-openapi.yml
- filename: apiman-developers-api-openapi.yml
  format: yaml
  label: Apiman Developers API
  slug: apiman-developers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-developers-api-openapi.yml
- filename: apiman-devportal-api-openapi.yml
  format: yaml
  label: Apiman Devportal API
  slug: apiman-devportal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-devportal-api-openapi.yml
- filename: apiman-downloads-api-openapi.yml
  format: yaml
  label: Apiman Downloads API
  slug: apiman-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-downloads-api-openapi.yml
- filename: apiman-events-api-openapi.yml
  format: yaml
  label: Apiman Events API
  slug: apiman-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-events-api-openapi.yml
- filename: apiman-experimental-api-openapi.yml
  format: yaml
  label: Apiman Experimental API
  slug: apiman-experimental-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-experimental-api-openapi.yml
- filename: apiman-gateways-api-openapi.yml
  format: yaml
  label: Apiman Gateways API
  slug: apiman-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-gateways-api-openapi.yml
- filename: apiman-organizations-api-openapi.yml
  format: yaml
  label: Apiman Organizations API
  slug: apiman-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-organizations-api-openapi.yml
- filename: apiman-plugins-api-openapi.yml
  format: yaml
  label: Apiman Plugins API
  slug: apiman-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-plugins-api-openapi.yml
- filename: apiman-policy-definitions-api-openapi.yml
  format: yaml
  label: Apiman Policy Definitions API
  slug: apiman-policy-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-policy-definitions-api-openapi.yml
- filename: apiman-roles-api-openapi.yml
  format: yaml
  label: Apiman Roles API
  slug: apiman-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-roles-api-openapi.yml
- filename: apiman-search-api-openapi.yml
  format: yaml
  label: Apiman Search API
  slug: apiman-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-search-api-openapi.yml
- filename: apiman-system-api-openapi.yml
  format: yaml
  label: Apiman System API
  slug: apiman-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-system-api-openapi.yml
- filename: apiman-users-api-openapi.yml
  format: yaml
  label: Apiman Users API
  slug: apiman-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/openapi/apiman-users-api-openapi.yml
auth_types:
- openIdConnect
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Apiman Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: Apiman secures its APIs with openIdConnect and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: Apiman
provider_slug: apiman
scheme_count: 3
schemes:
- applies_to: Apiman Manager REST API and Manager UI
  configuration:
  - description: Keycloak auth server URL (required)
    env: APIMAN_AUTH_URL
    property: apiman.auth.url
  - description: Keycloak realm name (default `apiman`)
    env: APIMAN_AUTH_REALM
    property: apiman.auth.realm
  - description: Client secret for the `apiman` Manager API client (default must be changed before production)
    env: APIMAN_AUTH_API_SECRET
    property: apiman.auth.api.secret
  - description: Client secret for the `apimanui` Manager UI client
    env: APIMAN_AUTH_UI_SECRET
    property: apiman.auth.ui.secret
  - description: Client secret for the `apiman-gateway-api` Gateway API client
    env: APIMAN_AUTH_GATEWAY_SECRET
    property: apiman.auth.gateway.secret
  - description: Realm public key. Only needed on the Vert.x gateway; otherwise Apiman retrieves it from the Keycloak server's .well-known endpoint automatically.
    env: APIMAN_AUTH_REALM_PUBLIC_KEY
    property: apiman.auth.realm-public-key
  description: 'The Manager REST API is protected by Keycloak (OIDC). Apiman 3 no longer bundles a Keycloak server; the operator runs one and points Apiman at it. Keycloak clients: `apiman` (Manager API), `apimanui` (Manager UI), `apiman-gateway-api` (Gateway API). Default realm name is `apiman`; the realm definition ships in the distribution as apiman/data/apiman-realm-for-keycloak.json.'
  discovery: Keycloak's own OIDC discovery document (/realms/<realm>/.well-known/openid-configuration) on the operator's Keycloak host. Apiman itself serves no discovery document — see well-known/apiman-well-known.yml.
  name: keycloakOidc
  sources:
  - https://www.apiman.io/apiman-docs/installation-guide/latest/keycloak.html
  type: openIdConnect
- applies_to: Apiman Gateway configuration REST API (invoked by the Manager when publishing)
  description: '"This REST API should be protected, usually by BASIC authentication. By default, the Apiman Gateway REST API requires BASIC authentication credentials, as well as a role of apipublisher." Default quickstart user `apimanager` / `apiman123!` — documented development credentials that must be changed before production.'
  keycloak_client: apiman-gateway-api
  name: gatewayBasicAuth
  required_role: apipublisher
  scheme: basic
  sources:
  - https://www.apiman.io/apiman-docs/installation-guide/latest/gateway/security.html
  type: http
  unauthenticated_exception: /system/status on the Vert.x Gateway API is reachable without auth as of 3.1.2.Final, so health checks do not need credentials.
  vertx_config:
    flowType: PASSWORD
    requiredRole: realm:apipublisher
    resource: apiman-gateway-api
- applies_to: APIs published THROUGH the Apiman gateway (runtime traffic, not the Manager API)
  description: Apiman mints an API key per Client App version, retrieved with getClientApiKey and rotated with updateClientApiKey. Consumers present it to the gateway when calling a managed API under a contract. This authenticates the gateway's downstream consumers, NOT calls to the Manager REST API — do not confuse the two surfaces.
  name: managedApiKey
  operations:
  - getClientApiKey
  - updateClientApiKey
  - getApiRegistryJSON
  - getApiRegistryXML
  policy_plugin: io.apiman.plugins:apiman-plugins-apikey-policy
  sources:
  - openapi/apiman-organizations-api-openapi.yml
  type: apiKey
slug: apiman-authentication
source_filename: apiman-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: >-\n  https://www.apiman.io/apiman-docs/installation-guide/latest/keycloak.html,\n  https://www.apiman.io/apiman-docs/installation-guide/latest/gateway/security.html,\n  https://www.apiman.io/apiman-docs/user-guide/latest/crash-course/managing-apiman.html,\n  openapi/_original/apiman-openapi.json\ndocs: https://www.apiman.io/apiman-docs/installation-guide/latest/keycloak.html\nspec_gap: >-\n  The published OpenAPI (https://www.apiman.io/openapi.json, 3.0.1, 128 paths / 177\n  operations) declares NO components.securitySchemes and NO top-level security block, so\n  a mechanical derivation from the spec yields nothing. Everything below is read from the\n  provider's own installation and user guides. This is a real contract gap worth raising\n  with the project: an agent reading only the spec cannot tell that the entire Manager\n  API is authenticated.\nsummary:\n  types: [openIdConnect, http]\n  api_key_in: []\n  oauth2_flows:\
  \ [authorizationCode, password]\n  authorization_model: role-based (Keycloak realm roles + Apiman organization roles)\nschemes:\n- name: keycloakOidc\n  type: openIdConnect\n  applies_to: Apiman Manager REST API and Manager UI\n  description: >-\n    The Manager REST API is protected by Keycloak (OIDC). Apiman 3 no longer bundles a\n    Keycloak server; the operator runs one and points Apiman at it. Keycloak clients:\n    `apiman` (Manager API), `apimanui` (Manager UI), `apiman-gateway-api` (Gateway API).\n    Default realm name is `apiman`; the realm definition ships in the distribution as\n    apiman/data/apiman-realm-for-keycloak.json.\n  configuration:\n  - property: apiman.auth.url\n    env: APIMAN_AUTH_URL\n    description: Keycloak auth server URL (required)\n  - property: apiman.auth.realm\n    env: APIMAN_AUTH_REALM\n    description: Keycloak realm name (default `apiman`)\n  - property: apiman.auth.api.secret\n    env: APIMAN_AUTH_API_SECRET\n    description: Client secret for\
  \ the `apiman` Manager API client (default must be changed before production)\n  - property: apiman.auth.ui.secret\n    env: APIMAN_AUTH_UI_SECRET\n    description: Client secret for the `apimanui` Manager UI client\n  - property: apiman.auth.gateway.secret\n    env: APIMAN_AUTH_GATEWAY_SECRET\n    description: Client secret for the `apiman-gateway-api` Gateway API client\n  - property: apiman.auth.realm-public-key\n    env: APIMAN_AUTH_REALM_PUBLIC_KEY\n    description: >-\n      Realm public key. Only needed on the Vert.x gateway; otherwise Apiman retrieves it\n      from the Keycloak server's .well-known endpoint automatically.\n  discovery: >-\n    Keycloak's own OIDC discovery document (/realms/<realm>/.well-known/openid-configuration)\n    on the operator's Keycloak host. Apiman itself serves no discovery document — see\n    well-known/apiman-well-known.yml.\n  sources: [https://www.apiman.io/apiman-docs/installation-guide/latest/keycloak.html]\n- name: gatewayBasicAuth\n  type:\
  \ http\n  scheme: basic\n  applies_to: Apiman Gateway configuration REST API (invoked by the Manager when publishing)\n  description: >-\n    \"This REST API should be protected, usually by BASIC authentication. By default, the\n    Apiman Gateway REST API requires BASIC authentication credentials, as well as a role\n    of apipublisher.\" Default quickstart user `apimanager` / `apiman123!` — documented\n    development credentials that must be changed before production.\n  required_role: apipublisher\n  keycloak_client: apiman-gateway-api\n  vertx_config:\n    flowType: PASSWORD\n    requiredRole: \"realm:apipublisher\"\n    resource: apiman-gateway-api\n  unauthenticated_exception: >-\n    /system/status on the Vert.x Gateway API is reachable without auth as of 3.1.2.Final,\n    so health checks do not need credentials.\n  sources: [https://www.apiman.io/apiman-docs/installation-guide/latest/gateway/security.html]\n- name: managedApiKey\n  type: apiKey\n  applies_to: APIs published THROUGH\
  \ the Apiman gateway (runtime traffic, not the Manager API)\n  description: >-\n    Apiman mints an API key per Client App version, retrieved with getClientApiKey and\n    rotated with updateClientApiKey. Consumers present it to the gateway when calling a\n    managed API under a contract. This authenticates the gateway's downstream consumers,\n    NOT calls to the Manager REST API — do not confuse the two surfaces.\n  operations: [getClientApiKey, updateClientApiKey, getApiRegistryJSON, getApiRegistryXML]\n  policy_plugin: io.apiman.plugins:apiman-plugins-apikey-policy\n  sources: [openapi/apiman-organizations-api-openapi.yml]\nauthorization:\n  model: role-based\n  realm_roles:\n  - name: apipublisher\n    description: Required to invoke the Gateway configuration REST API.\n  - name: apiadmin\n    description: Apiman administrator (system administration section, gateways, plugins, policy definitions, roles).\n  organization_roles:\n  - name: Organization Owner\n    description: Automatically\
  \ granted to the creator of an organization; all permissions.\n  - name: API Developer\n    description: Plan view/edit/admin and API view/edit/admin.\n  - name: Client App Developer\n    description: Client App view/edit/admin only.\n  custom_roles: >-\n    Administrators can define arbitrary roles from the permission set (org/plan/API/client\n    view, edit, admin) in the Roles section of System Administration, and mark roles as\n    auto-granted on organization creation (RoleBean.autoGrant, at least one such role must exist).\n  discoverability: >-\n    Apiman also has an implicit read-permission system (\"discoverability\") analogous to a\n    public GitHub repository, letting non-members — including anonymous users — find and\n    subscribe to APIs. It is set per API version and per plan (ApiVersionBean.discoverability,\n    ApiPlanBean.discoverability).\n  inspection_operations: [getPermissionsForUser, getInfo, listMembers, grant, revoke, revokeAll]\n  no_scopes: >-\n    Apiman publishes\
  \ no OAuth scope reference. Authorization is expressed as Keycloak\n    realm roles plus Apiman's own organization-scoped permission grid, so scopes/ is\n    deliberately absent rather than empty.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiman/refs/heads/main/authentication/apiman-authentication.yml
summary_line: openIdConnect/http · 3 schemes
tags:
- API Gateway
- API Management
- Developer Portal
- Java
- Open-Source
- Policy Enforcement
- Self-Hosted
- Keycloak
---
