---
api_key_in: []
api_specs:
- filename: vitagroup-hip-ehrbase-openehr.json
  format: json
  label: HIP EHRbase openEHR REST API
  slug: hip-ehrbase-openehr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-hip-ehrbase-openehr.json
- filename: vitagroup-hip-ehrbase-admin.json
  format: json
  label: HIP EHRbase Admin API
  slug: hip-ehrbase-admin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-hip-ehrbase-admin.json
- filename: vitagroup-hip-ehrbase-item-tags.json
  format: json
  label: HIP EHRbase Item Tag Experimental API
  slug: hip-ehrbase-item-tags
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-hip-ehrbase-item-tags.json
- filename: vitagroup-hip-ehrbase-enterprise.yml
  format: yaml
  label: HIP EHRbase Enterprise API
  slug: hip-ehrbase-enterprise
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-hip-ehrbase-enterprise.yml
- filename: vitagroup-ehrbase-sandbox-live.json
  format: json
  label: EHRbase Sandbox (live springdoc api-docs)
  slug: ehrbase-sandbox-live
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/openapi/vitagroup-ehrbase-sandbox-live.json
auth_types:
- none
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Vitagroup Authentication
name_suffix: Authentication
oauth_flows: []
overview: vitagroup secures its APIs with none, http, and oauth2 across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: vitagroup
provider_slug: vitagroup
scheme_count: 0
schemes: []
slug: vitagroup-authentication
source_filename: vitagroup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://docs.ehrbase.org/docs/EHRbase/Explore/Security\ndocs: https://docs.ehrbase.org/docs/EHRbase/Explore/Security\nnote: >-\n  HIP EHRbase is customer-deployed software, so the authentication mechanism is chosen\n  by the operator at boot rather than fixed by the vendor. The published OpenAPI documents\n  therefore declare almost no securitySchemes (only the enterprise plugin spec declares\n  bearerAuth); the real auth contract is documented in prose on the EHRbase Security\n  page and is captured here. Derived scheme detail from the spec is preserved under\n  spec_declared[].\nsummary:\n  types:\n  - none\n  - http\n  - oauth2\n  default_mode: none\n  selected_by: operator at startup via SECURITY_AUTHTYPE / security.authType\nmodes:\n- id: NONE\n  value: NONE\n  type: none\n  default: true\n  description: >-\n    EHRbase starts with security disabled by default and reports this in a boot message.\n    All resources are\
  \ reachable unauthenticated. This is the mode the public sandbox\n    at sandkiste.ehrbase.org runs in.\n  source: https://docs.ehrbase.org/docs/EHRbase/Explore/Security\n- id: BASIC\n  value: BASIC\n  type: http\n  scheme: basic\n  description: >-\n    A predefined set of users and roles configured at startup. Clients send\n    Authorization: Basic {base64(username:password)}.\n  configuration:\n  - env: SECURITY_AUTHTYPE\n    property: security.authType\n    value: BASIC\n  - env: SECURITY_AUTHUSER\n    property: security.authUser\n    default: ehrbase-user\n  - env: SECURITY_AUTHPASSWORD\n    property: security.authPassword\n    note: vendor default is a placeholder and must be replaced\n  - env: SECURITY_AUTHADMINUSER\n    property: security.authAdminUser\n    default: ehrbase-admin\n  - env: SECURITY_AUTHADMINPASSWORD\n    property: security.authAdminPassword\n    note: vendor default is a placeholder and must be replaced\n  source: https://docs.ehrbase.org/docs/EHRbase/Explore/Security\n\
  - id: OAUTH\n  value: OAUTH\n  type: oauth2\n  subtype: bearer JWT / OAuth 2.0 resource server\n  description: >-\n    EHRbase acts as an OAuth 2.0 resource server against an external authorization\n    server realm (Keycloak in the HIP platform). It validates the JWT and reads the\n    role claim to decide user vs admin access.\n  token_location: Authorization header, Bearer scheme\n  claims_read:\n  - realm_access.roles\n  - scope\n  configuration:\n  - env: SECURITY_AUTHTYPE\n    property: security.authType\n    value: OAUTH\n  - env: SPRING_SECURITY_OAUTH2_RESOURCESERVER_JWT_ISSUERURI\n    property: spring.security.oauth2.resourceserver.jwt.issuer-uri\n    description: base URL of the external authorization server realm\n    default: http://localhost:8081/auth/realms/ehrbase\n  - env: SECURITY_OAUTH2USERROLE\n    property: security.oauth2UserRole\n    default: USER\n  - env: SECURITY_OAUTH2ADMINROLE\n    property: security.oauth2AdminRole\n    default: ADMIN\n  source: https://docs.ehrbase.org/docs/EHRbase/Explore/Security\n\
  spec_declared:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  applies_to: HIP EHRbase Enterprise API (all operations)\n  sources:\n  - openapi/vitagroup-hip-ehrbase-enterprise.yml\nroles:\n- name: user\n  configurable_via: SECURITY_OAUTH2USERROLE\n  default: USER\n  grants: the standard openEHR REST surface\n- name: admin\n  configurable_via: SECURITY_OAUTH2ADMINROLE\n  default: ADMIN\n  grants: >-\n    the Admin API (/rest/admin/**), the Merge EHR operations, and by default the\n    Spring Actuator management endpoints\nmanagement_endpoint_access:\n  property: management.endpoints.web.access\n  values:\n  - ADMIN_ONLY\n  - PRIVATE\n  - PUBLIC\n  default: ADMIN_ONLY\n  csrf: >-\n    Write access to management endpoints is CSRF-protected by default; disable with\n    ehrbase.security.management.endpoints.web.csrf-validation-enabled=false\n  source: https://docs.ehrbase.org/docs/EHRbase/Explore/Status-And-Metrics\nmulti_tenancy:\n  supported: true\n  mechanism: >-\n    Tenants map\
  \ to Keycloak realms; data is logically separated with a dedicated\n    database schema per tenant. The enterprise Multi-tenant plugin API requires a\n    tenant user bearer token.\n  source: https://docs.ehrbase.org/docs/EHRbase/Enterprise-Features/Multi-Tenancy\ngaps:\n- The three open-source OpenAPI documents (openEHR, Admin, Item Tags) declare no\n  securitySchemes at all, so a generated client cannot tell from the contract that\n  Basic or Bearer auth may be required.\n- No OpenID Connect discovery document is published by vitagroup; the issuer is\n  operator-supplied per deployment.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vitagroup/refs/heads/main/authentication/vitagroup-authentication.yml
summary_line: none/http/oauth2 · 0 schemes
tags:
- Company
- Healthcare
- Health IT
- Electronic Health Records
- openEHR
- FHIR
- Clinical Data Repository
- Interoperability
- Germany
- Open Source
---
