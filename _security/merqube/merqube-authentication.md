---
api_key_in: []
api_specs:
- filename: merqube-api-api-openapi.yml
  format: yaml
  label: MerQube API
  slug: merqube-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merqube/refs/heads/main/openapi/merqube-api-api-openapi.yml
- filename: merqube-helper-api-openapi.yml
  format: yaml
  label: MerQube Helper API
  slug: merqube-helper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merqube/refs/heads/main/openapi/merqube-helper-api-openapi.yml
- filename: merqube-identifier-api-openapi.yml
  format: yaml
  label: MerQube Identifier API
  slug: merqube-identifier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merqube/refs/heads/main/openapi/merqube-identifier-api-openapi.yml
- filename: merqube-index-api-openapi.yml
  format: yaml
  label: MerQube Index API
  slug: merqube-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merqube/refs/heads/main/openapi/merqube-index-api-openapi.yml
- filename: merqube-legacy-equity-security-api-openapi.yml
  format: yaml
  label: MerQube Legacy Equity Security API
  slug: merqube-legacy-equity-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merqube/refs/heads/main/openapi/merqube-legacy-equity-security-api-openapi.yml
- filename: merqube-options-api-openapi.yml
  format: yaml
  label: MerQube Options API
  slug: merqube-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merqube/refs/heads/main/openapi/merqube-options-api-openapi.yml
- filename: merqube-portfolio-handler-api-openapi.yml
  format: yaml
  label: MerQube Portfolio Handler API
  slug: merqube-portfolio-handler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merqube/refs/heads/main/openapi/merqube-portfolio-handler-api-openapi.yml
- filename: merqube-security-api-openapi.yml
  format: yaml
  label: MerQube Security API
  slug: merqube-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merqube/refs/heads/main/openapi/merqube-security-api-openapi.yml
- filename: merqube-security-list-api-openapi.yml
  format: yaml
  label: MerQube Security List API
  slug: merqube-security-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/merqube/refs/heads/main/openapi/merqube-security-list-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Merqube Authentication
name_suffix: Authentication
oauth_flows: []
overview: MerQube declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MerQube
provider_slug: merqube
scheme_count: 1
schemes:
- description: 'Every MerQube API key is bound to a User. Requests carry the key in the Authorization header with the literal prefix "APIKEY " (note: not Bearer). Requests sent with no key are accepted but are treated as anonymous.'
  in: header
  name: apiKeyAuth
  parameter: Authorization
  source: https://merqube.stoplight.io/docs/api/p6s6m4p35ehfv-authentication
  type: apiKey
  value_format: APIKEY {your_api_key}
slug: merqube-authentication
source_filename: merqube-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: searched\nsource: >-\n  https://merqube.stoplight.io/docs/api/p6s6m4p35ehfv-authentication (MerQube's own Authentication\n  document), corroborated by\n  https://github.com/merqube/merqube-client-lib/blob/main/docs/Overview.md\ndocs: https://merqube.stoplight.io/docs/api/p6s6m4p35ehfv-authentication\nprovider: MerQube\nspec_declares_security: false\nspec_note: >-\n  The published OpenAPI (https://api.merqube.com/api, info.version 4.40.0) declares NO\n  components.securitySchemes and no top-level or per-operation `security` block, so the scheme below\n  is read from MerQube's prose Authentication document rather than derived from the contract. This\n  is a real contract gap: an agent reading only the OpenAPI cannot discover how to authenticate.\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  value_format: 'APIKEY {your_api_key}'\n  description: >-\n    Every MerQube API key is bound to a User. Requests\
  \ carry the key in the Authorization header\n    with the literal prefix \"APIKEY \" (note: not Bearer). Requests sent with no key are accepted but\n    are treated as anonymous.\n  source: https://merqube.stoplight.io/docs/api/p6s6m4p35ehfv-authentication\nkey_provisioning:\n  self_serve: false\n  steps:\n  - Create an account at https://merqube.com/register (company email address where applicable).\n  - Email support@merqube.com requesting an API key, stating the registration email and the intended\n    use so the correct permissions can be configured.\n  - MerQube emails a one-time-use link that reveals the key once; the key is not recoverable\n    afterwards by the customer or by MerQube.\n  contact: support@merqube.com\n  note: >-\n    Key issuance is human-gated - there is no self-service key creation in the public flow. The SDK\n    Overview additionally names an /apikey endpoint for key management, which is not present in the\n    published OpenAPI paths.\nauthorization_model:\n\
  \  style: namespace-scoped permissions\n  anonymous_access: true\n  anonymous_scope: >-\n    Unauthenticated callers receive only world-readable resources - everything in the `default`\n    namespace, which is where MerQube-branded public indices live (e.g. the MerQube US Index Series).\n  authenticated_scope: >-\n    An API key resolves to the union of the `default` namespace and every customer namespace the key\n    is permissioned for. Objects carry `namespace` and permissioning is applied per namespace, not\n    per object.\n  scopes_published: false\n  scopes_note: >-\n    No OAuth 2.0 scopes exist. Namespaces are the authorization primitive and MerQube does not\n    publish the namespace list; access changes are requested from support@merqube.com.\n  source: https://github.com/merqube/merqube-client-lib/blob/main/docs/Overview.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merqube/refs/heads/main/authentication/merqube-authentication.yml
summary_line: 1 scheme
tags:
- company
- Financial-Services
- index-data
- Market Data
- capital-markets
- investment-strategies
- asset-management
- ETFs
- structured-products
- quantitative-finance
- OpenAPI
---
