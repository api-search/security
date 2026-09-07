---
anonymous_access: false
api_key_in: []
api_specs:
- filename: viridi-parente-vista-openapi.json
  format: json
  label: Viridi ViSTA Platform API
  slug: viridi-parente-vista
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/viridi-parente/refs/heads/main/openapi/viridi-parente-vista-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Viridi Parente Authentication
name_suffix: Authentication
oauth_flows: []
overview: Viridi secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Viridi
provider_slug: viridi-parente
scheme_count: 3
schemes:
- bearerFormat: /api/auth/login|X-Authorization
  description: Enter Username / Password
  detail: 'The declared securityScheme. POST /api/auth/login exchanges username/password for a JWT; the token is presented on every subsequent call as `X-Authorization: Bearer <jwt>`, not as a standard Authorization header. POST /api/auth/token refreshes it; POST /api/auth/logout revokes it.'
  name: HTTP login form
  scheme: loginPassword
  sources:
  - openapi/viridi-parente-vista-openapi.json
  type: http
- declared_in_spec: false
  detail: Not declared in components.securitySchemes but demonstrably live. POST /api/noauth/oauth2Clients returns HTTP 200 anonymously with three configured identity providers — one Google provider and two enterprise providers (an Okta tenant and an ADFS tenant) — each with an /oauth2/authorization/<uuid> entry URL. The contract carries an o-auth-2-controller and an o-auth-2-config-template-controller (GET/POST /api/oauth2/config, GET /api/oauth2/config/template, GET /api/oauth2/loginProcessingUrl).
  evidence:
    method: POST
    providers_configured: 3
    status: 200
    url: https://vista.viridiparente.com/api/noauth/oauth2Clients
  method: probed
  name: OAuth2 / OIDC single sign-on
  type: oauth2
- declared_in_spec: false
  detail: 'two-factor-auth-controller and two-factor-auth-config-controller are present: GET /api/auth/2fa/providers, POST /api/auth/2fa/verification/send, POST /api/auth/2fa/verification/check.'
  name: Two-factor authentication
  type: mfa
slug: viridi-parente-authentication
source_filename: viridi-parente-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: openapi/viridi-parente-vista-openapi.json + live probes of https://vista.viridiparente.com (2026-09-04)\ndocs: https://vista.viridiparente.com/swagger-ui/index.html\nsummary:\n  types:\n  - http\n  - oauth2\n  primary: bearer JWT in the X-Authorization header\n  self_service_signup: false\n  signup: https://viridiparente.com/create-a-vista-account/\nschemes:\n- name: HTTP login form\n  type: http\n  scheme: loginPassword\n  bearerFormat: /api/auth/login|X-Authorization\n  description: Enter Username / Password\n  sources:\n  - openapi/viridi-parente-vista-openapi.json\n  detail: >-\n    The declared securityScheme. POST /api/auth/login exchanges username/password for a JWT;\n    the token is presented on every subsequent call as `X-Authorization: Bearer <jwt>`, not\n    as a standard Authorization header. POST /api/auth/token refreshes it; POST\n    /api/auth/logout revokes it.\n- name: OAuth2 / OIDC single sign-on\n  type:\
  \ oauth2\n  declared_in_spec: false\n  method: probed\n  detail: >-\n    Not declared in components.securitySchemes but demonstrably live. POST\n    /api/noauth/oauth2Clients returns HTTP 200 anonymously with three configured identity\n    providers — one Google provider and two enterprise providers (an Okta tenant and an\n    ADFS tenant) — each with an /oauth2/authorization/<uuid> entry URL. The contract carries\n    an o-auth-2-controller and an o-auth-2-config-template-controller\n    (GET/POST /api/oauth2/config, GET /api/oauth2/config/template,\n    GET /api/oauth2/loginProcessingUrl).\n  evidence:\n    url: https://vista.viridiparente.com/api/noauth/oauth2Clients\n    method: POST\n    status: 200\n    providers_configured: 3\n- name: Two-factor authentication\n  type: mfa\n  declared_in_spec: false\n  detail: >-\n    two-factor-auth-controller and two-factor-auth-config-controller are present:\n    GET /api/auth/2fa/providers, POST /api/auth/2fa/verification/send, POST\n    /api/auth/2fa/verification/check.\n\
  scopes:\n  published: false\n  note: >-\n    No OAuth2 scope surface. Authorization is role- and tenant-based rather than\n    scope-based: the contract exposes a role-controller, and every entity carries tenantId /\n    customerId, with 401 returned when \"User belongs to different Customer or Tenant\".\n    scopes/ is deliberately not written for this provider.\ndevice_transport_auth:\n  note: >-\n    Device-side credentials are managed through device-controller and device-profile\n    transport configuration (access token, X.509, MQTT basic, LwM2M). The CBRS surface adds\n    Viridi-authored certificate operations, GET /api/getCert and POST /api/setCert.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/viridi-parente/refs/heads/main/authentication/viridi-parente-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Company
- Energy
- Energy Storage
- Battery
- IoT
- Industrial IoT
- Energy Management
- Manufacturing
- Telematics
- Microgrid
---
