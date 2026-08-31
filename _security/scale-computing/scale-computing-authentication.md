---
api_key_in:
- header
api_specs:
- filename: scale-computing-api-keys-api-openapi.yml
  format: yaml
  label: Scale Computing API Keys API
  slug: scale-computing-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-api-keys-api-openapi.yml
- filename: scale-computing-clusters-api-openapi.yml
  format: yaml
  label: Scale Computing Clusters API
  slug: scale-computing-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-clusters-api-openapi.yml
- filename: scale-computing-conditions-api-openapi.yml
  format: yaml
  label: Scale Computing Conditions API
  slug: scale-computing-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-conditions-api-openapi.yml
- filename: scale-computing-health-api-openapi.yml
  format: yaml
  label: Scale Computing Health API
  slug: scale-computing-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-health-api-openapi.yml
- filename: scale-computing-metrics-api-openapi.yml
  format: yaml
  label: Scale Computing Metrics API
  slug: scale-computing-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-metrics-api-openapi.yml
- filename: scale-computing-nodes-api-openapi.yml
  format: yaml
  label: Scale Computing Nodes API
  slug: scale-computing-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-nodes-api-openapi.yml
- filename: scale-computing-organization-activities-api-openapi.yml
  format: yaml
  label: Scale Computing Organization Activities API
  slug: scale-computing-organization-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organization-activities-api-openapi.yml
- filename: scale-computing-organization-api-openapi.yml
  format: yaml
  label: Scale Computing Organization API
  slug: scale-computing-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organization-api-openapi.yml
- filename: scale-computing-organization-salesforce-account-api-openapi.yml
  format: yaml
  label: Scale Computing Organization Salesforce Account API
  slug: scale-computing-organization-salesforce-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organization-salesforce-account-api-openapi.yml
- filename: scale-computing-organizationroles-api-openapi.yml
  format: yaml
  label: Scale Computing Organization Roles API
  slug: scale-computing-organizationroles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organizationroles-api-openapi.yml
- filename: scale-computing-organizations-api-openapi.yml
  format: yaml
  label: Scale Computing Organizations API
  slug: scale-computing-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organizations-api-openapi.yml
- filename: scale-computing-organizationuser-api-openapi.yml
  format: yaml
  label: Scale Computing Organization User API
  slug: scale-computing-organizationuser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organizationuser-api-openapi.yml
- filename: scale-computing-organizationusers-api-openapi.yml
  format: yaml
  label: Scale Computing Organization Users API
  slug: scale-computing-organizationusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-organizationusers-api-openapi.yml
- filename: scale-computing-salesforce-api-openapi.yml
  format: yaml
  label: Scale Computing Salesforce API
  slug: scale-computing-salesforce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-salesforce-api-openapi.yml
- filename: scale-computing-staged-clusters-api-openapi.yml
  format: yaml
  label: Scale Computing Staged Clusters API
  slug: scale-computing-staged-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-staged-clusters-api-openapi.yml
- filename: scale-computing-users-api-openapi.yml
  format: yaml
  label: Scale Computing Users API
  slug: scale-computing-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-users-api-openapi.yml
- filename: scale-computing-vms-api-openapi.yml
  format: yaml
  label: Scale Computing Vms API
  slug: scale-computing-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/openapi/scale-computing-vms-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Scale Computing Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scale Computing secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Scale Computing
provider_slug: scale-computing
scheme_count: 3
schemes:
- api: SC//Fleet Manager API
  applied_to: Every operation in the v2 spec except HealthController_check, via a per-operation security requirement.
  authorization_model: role
  created_via_api: POST /api/v2/api-keys (ApiKeyController_create)
  in: header
  issued_at: https://fleet.scalecomputing.com/organization/settings
  key_metadata: ApiKeyDto exposes id, name, organizationId, tokenSuffix, role, createdAt, lastUsed
  name: API Key
  parameter: api-key
  revoked_via_api: DELETE /api/v2/api-keys/{id} (ApiKeyController_remove) — irreversible
  roles_enumerated: false
  roles_note: The published description states "Each endpoint is role restricted in alignment with the UI access levels, which are detailed in the Fleet Manager User Guide". The role vocabulary is NOT in the spec — the only role named anywhere in the contract is "VM Viewer", in the CreateApiKeyDto example payload — and the User Guide is a Salesforce-hosted content link, so the authoritative permission matrix is not machine-readable and is effectively customer-gated.
  rotation: No rotation endpoint and no expiry field. Rotation means create-then-revoke, which the caller must sequence themselves; there is no overlap or grace window published.
  sources:
  - openapi/scale-computing-fleet-manager-openapi.json
  transport_security: TLS 1.3; HSTS max-age=31536000; includeSubDomains observed on api.scalecomputing.com
  type: apiKey
- api: Scale Computing Platform Core API
  flows:
  - authorizationUrl: http://swagger.io/api/oauth/dialog
    flow: implicit
    scopes: 0
  name: tsoa_auth
  note: NOT a real Scale Computing authorization server. This is the stock tsoa scaffold placeholder — the authorization URL points at swagger.io's demo dialog over plain HTTP and the scope set is empty. Recorded so it is not mistaken for OAuth support. The v1 core API's actual credential flow is a bearer/session token minted by POST /api/v1/users/me/access-token (CreateAccessToken) and validated by GET /api/v1/users/me (AuthenticateUser), but no operation in the spec declares a security requirement and no documentation for it is published.
  sources:
  - openapi/scale-computing-core-openapi.json
  type: oauth2
  valid: false
- api: SC//HyperCore REST API
  name: on-appliance auth
  note: The HyperCore API is served by the customer's own clustered node, authenticated with cluster user credentials (the Ansible collection and Terraform provider take a host, username and password). No machine-readable contract for it is published outside the customer network, so this entry is recorded from the first-party tooling rather than from a spec.
  scheme: basic
  sources:
  - https://scalecomputing.github.io/HyperCoreAnsibleCollection/
  type: http
slug: scale-computing-authentication
source_filename: scale-computing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: >-\n  https://api.scalecomputing.com/api/v2 (Swagger UI description),\n  openapi/scale-computing-fleet-manager-openapi.json, openapi/scale-computing-core-openapi.json\ndocs: https://api.scalecomputing.com/api/v2\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    The only genuine authentication mechanism Scale Computing publishes for a reachable API is an\n    API key sent in an `api-key` request header. There is no OAuth 2.0, no OIDC and no scope model.\nschemes:\n- name: API Key\n  api: SC//Fleet Manager API\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/scale-computing-fleet-manager-openapi.json\n  applied_to: >-\n    Every operation in the v2 spec except HealthController_check, via a per-operation\n    security requirement.\n  issued_at: https://fleet.scalecomputing.com/organization/settings\n  created_via_api: 'POST /api/v2/api-keys (ApiKeyController_create)'\n\
  \  revoked_via_api: 'DELETE /api/v2/api-keys/{id} (ApiKeyController_remove) — irreversible'\n  key_metadata: 'ApiKeyDto exposes id, name, organizationId, tokenSuffix, role, createdAt, lastUsed'\n  rotation: >-\n    No rotation endpoint and no expiry field. Rotation means create-then-revoke, which the caller\n    must sequence themselves; there is no overlap or grace window published.\n  authorization_model: role\n  roles_enumerated: false\n  roles_note: >-\n    The published description states \"Each endpoint is role restricted in alignment with the UI access\n    levels, which are detailed in the Fleet Manager User Guide\". The role vocabulary is NOT in the\n    spec — the only role named anywhere in the contract is \"VM Viewer\", in the CreateApiKeyDto example\n    payload — and the User Guide is a Salesforce-hosted content link, so the authoritative permission\n    matrix is not machine-readable and is effectively customer-gated.\n  transport_security: 'TLS 1.3; HSTS max-age=31536000;\
  \ includeSubDomains observed on api.scalecomputing.com'\n- name: tsoa_auth\n  api: Scale Computing Platform Core API\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: http://swagger.io/api/oauth/dialog\n    scopes: 0\n  sources:\n  - openapi/scale-computing-core-openapi.json\n  valid: false\n  note: >-\n    NOT a real Scale Computing authorization server. This is the stock tsoa scaffold placeholder — the\n    authorization URL points at swagger.io's demo dialog over plain HTTP and the scope set is empty.\n    Recorded so it is not mistaken for OAuth support. The v1 core API's actual credential flow is a\n    bearer/session token minted by POST /api/v1/users/me/access-token (CreateAccessToken) and validated\n    by GET /api/v1/users/me (AuthenticateUser), but no operation in the spec declares a security\n    requirement and no documentation for it is published.\n- name: on-appliance auth\n  api: SC//HyperCore REST API\n  type: http\n  scheme: basic\n  sources:\n  - https://scalecomputing.github.io/HyperCoreAnsibleCollection/\n\
  \  note: >-\n    The HyperCore API is served by the customer's own clustered node, authenticated with cluster user\n    credentials (the Ansible collection and Terraform provider take a host, username and password).\n    No machine-readable contract for it is published outside the customer network, so this entry is\n    recorded from the first-party tooling rather than from a spec.\nx-negative-results:\n- probe: https://api.scalecomputing.com/.well-known/oauth-authorization-server\n  status: 404\n- probe: https://api.scalecomputing.com/.well-known/openid-configuration\n  status: 404\n- probe: https://community.scalecomputing.com/.well-known/openid-configuration\n  status: 200\n  finding: >-\n    Real OIDC discovery document, but it is Salesforce Experience Cloud's issuer for the customer\n    community portal (issuer https://community.scalecomputing.com, stock Salesforce scope list). It\n    does not authorize either Scale Computing API. See well-known/scale-computing-well-known.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scale-computing/refs/heads/main/authentication/scale-computing-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- edge-computing
- hyperconverged-infrastructure
- Virtualization
- infrastructure-management
- fleet-management
- virtual-machines
- observability
- infrastructure-as-code
- kubernetes
---
