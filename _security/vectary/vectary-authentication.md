---
api_key_in: []
auth_types: []
description: 'Access model for Vectary''s developer surface. Vectary publishes no REST API and no OpenAPI, so there are no securitySchemes to derive — this profile is captured from the Model API documentation. Access to the Model API is plan-gated rather than credential-gated: the VctrModelApi browser script is provided to Business-plan workspaces, and an embed is addressed by its public Project ID (the UUID in the https://app.vectary.com/p/<id> embed URL). No API keys, tokens, or OAuth flows are documented for the Model API. Platform account access supports SSO and RBAC on Enterprise plans.'
kind: authentication
layout: security
method: searched
name: Vectary Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vectary declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Vectary
provider_slug: vectary
scheme_count: 1
schemes:
- description: Model API availability requires a Business plan workspace; the api.js script (VctrModelApi) is initialized against the iframe's DOM id and communicates with the embedded scene over postMessage. The Project ID from the share/embed URL identifies the scene.
  docs: https://help.vectary.com/api/model-api
  name: business-plan-gate
  type: plan-gated
slug: vectary-authentication
source_filename: vectary-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://help.vectary.com/api/model-api\ndocs: https://help.vectary.com/api/model-api/quick-start\ndescription: >-\n  Access model for Vectary's developer surface. Vectary publishes no REST API\n  and no OpenAPI, so there are no securitySchemes to derive — this profile is\n  captured from the Model API documentation. Access to the Model API is\n  plan-gated rather than credential-gated: the VctrModelApi browser script is\n  provided to Business-plan workspaces, and an embed is addressed by its\n  public Project ID (the UUID in the https://app.vectary.com/p/<id> embed\n  URL). No API keys, tokens, or OAuth flows are documented for the Model API.\n  Platform account access supports SSO and RBAC on Enterprise plans.\nsummary:\n  types: []\n  model: plan-gated embed script (no API credentials)\nschemes:\n  - name: business-plan-gate\n    type: plan-gated\n    description: >-\n      Model API availability requires a Business plan\
  \ workspace; the api.js\n      script (VctrModelApi) is initialized against the iframe's DOM id and\n      communicates with the embedded scene over postMessage. The Project ID\n      from the share/embed URL identifies the scene.\n    docs: https://help.vectary.com/api/model-api\nenterprise:\n  sso: Single sign-on (SSO) available on Enterprise plans\n  rbac: Role-Based Access Control (RBAC) available on Enterprise plans\n  source: https://www.vectary.com/security/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectary/refs/heads/main/authentication/vectary-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Design Tech
- 3D Design
- Augmented Reality
- 3D Configurator
- Product Visualization
- ECommerce
---
