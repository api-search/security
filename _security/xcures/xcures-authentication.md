---
anonymous_access: false
api_key_in: []
api_specs:
- filename: xcures-patient-registry-api-openapi.yml
  format: yaml
  label: xCures Public API
  slug: xcures-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xcures/refs/heads/main/openapi/xcures-patient-registry-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Xcures Authentication
name_suffix: Authentication
oauth_flows: []
overview: xCures secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: xCures
provider_slug: xcures
scheme_count: 2
schemes:
- applied_to: 68 of 69 operations
  bearerFormat: JWT
  declared_at_document_level: false
  exempt:
  - PublicOAuthController_token
  header: Authorization
  name: bearer
  scheme: bearer
  sources:
  - openapi/xcures-patient-registry-api-openapi.yml
  type: http
- declared_in_docs: true
  declared_in_spec: false
  flow: clientCredentials
  name: oauth2-client-credentials
  operationId: PublicOAuthController_token
  request_fields:
  - client_id
  - client_secret
  - grant_type (value: client_credentials)
  request_media_type: application/json
  response_fields:
  - access_token
  - token_type
  scopes: {}
  scopes_note: 'NO SCOPES ARE PUBLISHED. The token response carries no scope, the token request accepts no scope parameter, and no scope reference page exists. Authorization is not scope-based here: it is the combination of (a) which projects a credential was granted in the portal and (b) the permissions selected on that credential at creation time, enforced through the ProjectId header. That is why no scopes/ artifact is emitted for this provider — an empty scope file would misrepresent the model.'
  sources:
  - https://docs.xcures.com/api-introduction#obtaining-a-bearer-token
  - openapi/xcures-patient-registry-api-openapi.yml (info.description)
  token_url: https://partner.xcures.com/oauth/token
  type: oauth2
slug: xcures-authentication
source_filename: xcures-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://docs.xcures.com/api-introduction#authentication (docs) enriched over a derive from\n  openapi/xcures-patient-registry-api-openapi.yml securitySchemes\ndocs: https://docs.xcures.com/api-introduction#authentication\napi: xCures Public API\nsummary:\n  types:\n    - http\n    - oauth2\n  note: >-\n    The spec declares only one securityScheme (http bearer, JWT), but the docs and the spec's own\n    info.description document the full OAuth 2.0 client-credentials exchange that mints that bearer.\n    Recorded as both: an implementer needs the grant, not just the header.\nschemes:\n  - name: bearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    header: Authorization\n    applied_to: 68 of 69 operations\n    exempt: [PublicOAuthController_token]\n    declared_at_document_level: false\n    sources:\n      - openapi/xcures-patient-registry-api-openapi.yml\n  - name: oauth2-client-credentials\n    type:\
  \ oauth2\n    flow: clientCredentials\n    token_url: https://partner.xcures.com/oauth/token\n    operationId: PublicOAuthController_token\n    request_media_type: application/json\n    request_fields:\n      - client_id\n      - client_secret\n      - grant_type (value: client_credentials)\n    response_fields:\n      - access_token\n      - token_type\n    scopes: {}\n    scopes_note: >-\n      NO SCOPES ARE PUBLISHED. The token response carries no scope, the token request accepts no scope\n      parameter, and no scope reference page exists. Authorization is not scope-based here: it is the\n      combination of (a) which projects a credential was granted in the portal and (b) the permissions\n      selected on that credential at creation time, enforced through the ProjectId header. That is why no\n      scopes/ artifact is emitted for this provider — an empty scope file would misrepresent the model.\n    declared_in_spec: false\n    declared_in_docs: true\n    sources:\n      - https://docs.xcures.com/api-introduction#obtaining-a-bearer-token\n\
  \      - openapi/xcures-patient-registry-api-openapi.yml (info.description)\nproject_context:\n  header: ProjectId\n  required: true\n  required_on: 67 of 69 operations\n  exempt:\n    - PublicOAuthController_token\n    - PublicProjectController_getAll\n  value: UUID of a project the credential has permission to access\n  discovery: GET /api/v1/patient-registry/project\n  failure_mode: >-\n    A missing or unauthorized ProjectId returns 401 (\"Invalid API key or ProjectId\"), not 400 or 403. This\n    is the most common integration mistake and the docs call it out first in the error table.\ncredential_lifecycle:\n  issuance: >-\n    Initial portal credentials come from a Customer Success Manager. API keys are then self-managed:\n    Administration > API Keys > + Add, naming the key, selecting the Projects it can reach and the\n    permissions it carries. The client_id and client_secret are shown once.\n  self_service: true\n  since: '2025-12-04'\n  deactivation: toggle the ACTIVE switch\
  \ on the credential (confirmation modal)\n  rotation: >-\n    Supported and documented as expected practice — open the credential and use Rotate at the bottom of\n    the page; new credentials are displayed on completion. xCures publishes a short rationale for\n    rotation in the docs.\n  legacy_cutover:\n    announced: '2025-12-04'\n    effective: '2026-01-31'\n    detail: >-\n      All credentials created before December 2025 were deactivated after 2026-01-31 and had to be\n      recreated with the self-service tool; they only ever worked against the previous (now undocumented)\n      OAuth endpoint.\n  handling_guidance_published: >-\n    \"Your client_id and client_secret are privileged. Do not share publicly, expose in your code\n    repository, or include in client-side code. This is extremely sensitive, given it may give access to\n    your organization's PHI.\"\ntoken:\n  format: JWT\n  lifetime_published: false\n  refresh: >-\n    None. The client-credentials grant returns no\
  \ refresh_token; re-run the exchange. The docs call the\n    result a \"temporary access token\" but publish no TTL.\n  revocation_endpoint: none published\n  introspection_endpoint: none published\ndiscovery_documents:\n  openid_configuration: none (404 on every host)\n  oauth_authorization_server: >-\n    Not served for the Public API. The document at\n    https://docs.xcures.com/.well-known/oauth-authorization-server belongs to the DOCS PORTAL / MCP login\n    (issuer https://auth.cloud.redocly.com) — see well-known/xcures-well-known.yml. Do not mistake it for\n    the API's OAuth server.\ngaps:\n  - No published token lifetime, so a client cannot pre-emptively refresh.\n  - No scopes and no scope reference, so least-privilege is expressed only in the portal UI.\n  - No mTLS, no signed requests, no IP allowlisting documented for a PHI-bearing API.\n  - No discovery document for the Public API's own authorization server.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xcures/refs/heads/main/authentication/xcures-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Health
- Healthcare
- Medical Records
- Interoperability
- FHIR
- Oncology
- Real World Data
- Clinical Data
- Artificial Intelligence
- TEFCA
- Carequality
- Patient Data
- HITRUST
- HIPAA
---
