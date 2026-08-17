---
api_key_in:
- header
- query
api_specs:
- filename: permutive-cohorts-api-openapi.yml
  format: yaml
  label: Permutive Cohorts API
  slug: permutive-cohorts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-cohorts-api-openapi.yml
- filename: permutive-contextual-api-openapi.yml
  format: yaml
  label: Permutive Contextual API
  slug: permutive-contextual-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-contextual-api-openapi.yml
- filename: permutive-events-api-openapi.yml
  format: yaml
  label: Permutive Events API
  slug: permutive-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-events-api-openapi.yml
- filename: permutive-identity-api-openapi.yml
  format: yaml
  label: Permutive Identity API
  slug: permutive-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-identity-api-openapi.yml
- filename: permutive-segmentation-api-openapi.yml
  format: yaml
  label: Permutive Segmentation API
  slug: permutive-segmentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-segmentation-api-openapi.yml
- filename: permutive-taxonomy-api-openapi.yml
  format: yaml
  label: Permutive Taxonomy API
  slug: permutive-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/openapi/permutive-taxonomy-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Permutive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Permutive secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Permutive
provider_slug: permutive
scheme_count: 2
schemes:
- description: Permutive API key (UUID v4) supplied in the X-API-Key request header. The CCS API spells the same header `X-Api-Key`; header names are case-insensitive per RFC 9110.
  in: header
  name: Header
  parameter: X-API-Key
  sources:
  - openapi/permutive-events-api-openapi.yml
  - openapi/permutive-identity-api-openapi.yml
  - openapi/permutive-segmentation-api-openapi.yml
  type: apiKey
- description: Permutive API key (UUID v4) supplied on the `k` query parameter. Documented as the primary mechanism for the Contextual API and as an alternative everywhere else. Note that keys on the query string are logged by intermediaries — prefer the header wherever you control the client.
  in: query
  name: Parameter
  parameter: k
  sources:
  - openapi/permutive-cohorts-api-openapi.yml
  - openapi/permutive-events-api-openapi.yml
  - openapi/permutive-identity-api-openapi.yml
  - openapi/permutive-segmentation-api-openapi.yml
  type: apiKey
slug: permutive-authentication
source_filename: permutive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.permutive.com/api/authentication\ndocs: https://docs.permutive.com/api/authentication\nspecs:\n- openapi/permutive-cohorts-api-openapi.yml\n- openapi/permutive-events-api-openapi.yml\n- openapi/permutive-identity-api-openapi.yml\n- openapi/permutive-segmentation-api-openapi.yml\nnotes: >-\n  CORRECTION to the 2026-07-20 profile, which recorded HTTP bearer auth. That\n  was derived from an API Evangelist-authored spec and was wrong. Permutive's\n  own documentation and its own five OpenAPI documents both state the model\n  plainly: authentication is an API KEY in the form of a version-4 UUID, passed\n  either in the `X-API-Key` request header or on the `k` query parameter. There\n  is no bearer token, no OAuth2 and no OIDC on the Permutive product API.\n  Keys come in two grades — PUBLIC keys for surfaces you cannot keep secret\n  (sites and apps) and PRIVATE keys for account mutation. The Cohorts API and\n  the\
  \ Taxonomy API accept private keys only. Client-side CCS integrations must\n  use a public key; server-side CCS integrations must use a private key.\n  Key provisioning is self-serve in the Permutive Dashboard under\n  Settings › Keys (https://dash.permutive.com/settings/keys).\nsummary:\n  types: [apiKey]\n  api_key_in: [header, query]\n  api_key_names: [X-API-Key, k]\n  key_format: UUID v4\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\nkey_types:\n- name: public\n  description: >-\n    Used where the key cannot be kept secret — typically embedded in the web,\n    mobile and CTV SDK deployments on your own properties.\n  used_for: [Events API, Identity API, Contextual API, 'CCS API (client-side)']\n- name: private\n  description: >-\n    Used where the key can be kept secret. Required for anything that changes\n    the Permutive account.\n  used_for: [Cohorts API, Taxonomy API, 'CCS API (server-side)']\n  access_levels: >-\n    A private key defaults to read-only access\
  \ to cohorts in the workspace that\n    owns it, plus cohorts inherited from parent workspaces. Broader access\n    levels are arranged with Permutive Technical Services\n    (technical-services@permutive.com).\nscopes_model:\n  kind: workspace\n  description: >-\n    Authorization is by workspace, not by OAuth scope. The behaviour of every\n    call depends on which workspace in the organization hierarchy owns the key;\n    the Cohorts API exposes an `include-child-workspaces` query parameter to\n    reach workspaces below the requesting one.\nschemes:\n- name: Header\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: >-\n    Permutive API key (UUID v4) supplied in the X-API-Key request header. The\n    CCS API spells the same header `X-Api-Key`; header names are\n    case-insensitive per RFC 9110.\n  sources:\n  - openapi/permutive-events-api-openapi.yml\n  - openapi/permutive-identity-api-openapi.yml\n  - openapi/permutive-segmentation-api-openapi.yml\n- name: Parameter\n\
  \  type: apiKey\n  in: query\n  parameter: k\n  description: >-\n    Permutive API key (UUID v4) supplied on the `k` query parameter. Documented\n    as the primary mechanism for the Contextual API and as an alternative\n    everywhere else. Note that keys on the query string are logged by\n    intermediaries — prefer the header wherever you control the client.\n  sources:\n  - openapi/permutive-cohorts-api-openapi.yml\n  - openapi/permutive-events-api-openapi.yml\n  - openapi/permutive-identity-api-openapi.yml\n  - openapi/permutive-segmentation-api-openapi.yml\ngaps:\n- >-\n  openapi/permutive-taxonomy-api-openapi.yml declares no securitySchemes at all,\n  although the Taxonomy API documentation states that every request must carry a\n  private API key. The spec understates the contract.\nsso:\n  platform_login: >-\n    The Permutive platform (dash.permutive.com) supports enterprise SSO via SAML\n    and OpenID Connect with MFA enforced through the customer IdP. This is\n    console\
  \ authentication for humans and is unrelated to API authentication.\n  source: https://docs.permutive.com/governance/security\ncross_links:\n  conventions: conventions/permutive-conventions.yml\n  errors: errors/permutive-problem-types.yml\n  key_management: https://dash.permutive.com/settings/keys\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/permutive/refs/heads/main/authentication/permutive-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Publishing
- Advertising
- AdTech
- MarTech
- Audience
- Data Collaboration
- Data Management Platform
- Contextual
- Identity
- Segmentation
- Agents
---
