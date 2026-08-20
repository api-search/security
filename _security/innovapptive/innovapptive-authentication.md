---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Innovapptive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Innovapptive secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Innovapptive
provider_slug: innovapptive
scheme_count: 2
schemes:
- description: Tenant-scoped API key issued by the Innovapptive security module. The Swagger console exposes it through the Authorize dialog ("enter the API Key value and click Authorize"). A request without the header, or with an invalid/expired key, is rejected with HTTP 401.
  in: header
  name: ApiKeyAuth
  parameter_name: x-api-key
  source: docs
  type: apiKey
- description: Mandatory tenant discriminator accompanying every external Operator Rounds request; the value is the Tenant ID created by CBO Tenant Management. A missing/unknown value is rejected with HTTP 401 ("TenantId <x> not found in db or cache"). Documented as a request parameter on every operation, so it is a de-facto second credential dimension rather than an ordinary filter.
  in: header
  name: TenantId
  parameter_name: tenantid
  required: true
  source: docs
  type: apiKey
slug: innovapptive-authentication
source_filename: innovapptive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: >-\n  https://docs.innovapptive.com/2605/mRounds_configuration_guide/html/topics/api_using_overview.html\ndocs:\n- https://docs.innovapptive.com/2605/mRounds_configuration_guide/html/topics/api_using_overview.html\n- https://docs.innovapptive.com/2605/mRounds_configuration_guide/html/topics/api_keys_generate_overview.html\n- https://docs.innovapptive.com/2605/mRounds_configuration_guide/html/topics/api_generate_key.html\n- https://docs.innovapptive.com/2605/mRounds_configuration_guide/html/topics/api_keys_generate_prerequisites.html\nnote: >-\n  Derived from the published documentation, not from a machine-readable spec —\n  Innovapptive publishes a Swagger UI console for the external Operator Rounds API\n  but does not expose the underlying OpenAPI document anonymously (see\n  spec_discovery below).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n\
  schemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    Tenant-scoped API key issued by the Innovapptive security module. The Swagger\n    console exposes it through the Authorize dialog (\"enter the API Key value and\n    click Authorize\"). A request without the header, or with an invalid/expired\n    key, is rejected with HTTP 401.\n  source: docs\n- name: TenantId\n  type: apiKey\n  in: header\n  parameter_name: tenantid\n  required: true\n  description: >-\n    Mandatory tenant discriminator accompanying every external Operator Rounds\n    request; the value is the Tenant ID created by CBO Tenant Management. A\n    missing/unknown value is rejected with HTTP 401 (\"TenantId <x> not found in db\n    or cache\"). Documented as a request parameter on every operation, so it is a\n    de-facto second credential dimension rather than an ordinary filter.\n  source: docs\nkey_lifecycle:\n  issued_by: CBO application, Tenant Management\
  \ module, API Keys tab\n  issued_during: tenant onboarding, or on customer request for programmatic access\n  issuer_role: CBO admin / Tenant Admin\n  fields:\n  - description\n  - expires\n  expiry_options_days:\n  - 30\n  - 90\n  - 180\n  - 365\n  rotation: >-\n    Keys are generated with a fixed expiry and revoked by deleting them from the\n    API Keys tab (More icon > Delete). No self-service developer key management is\n    published.\n  self_service: false\nscope_model:\n  scopes: none\n  note: >-\n    No OAuth2 scope surface is published for the external API. Authorization is\n    coarse — a key is bound to a tenant and to \"the set of APIs identified as being\n    programmatically accessed by a tenant\". Fine-grained access inside the product\n    is handled by CBO roles/permissions, not by API scopes.\nrestrictions:\n- >-\n  API-key access is explicitly restricted to programmatic consumers. Innovapptive's\n  own web and mobile clients cannot use it — \"If any application consumes\
  \ the same\n  API, they should follow the traditional token-based authentication mechanism.\"\nother_auth_surfaces:\n- name: Token-based application authentication\n  applies_to: Innovapptive web and mobile clients (iMaintenance, iPermits, mRounds)\n  docs: https://docs.innovapptive.com/2607/imaintenance_configuration_guide/html/imaintenance_configuration_guide/topics/token_based_app_api_flow.html\n  note: Customer-configured; not an externally callable credential.\n- name: SAP BTP API Management OAuth 2.0\n  applies_to: >-\n    Customer-deployed SAP integration layer (OAuth token proxy, OAuth v2.0 policies\n    to generate and verify access tokens between an external consumer and BTP API\n    Management)\n  docs: https://docs.innovapptive.com/2607/imaintenance_deployment_setup_guide/html/imaintenance_deployment_setup_guide/topics/sap_oauth_api_proxy.html\n  note: >-\n    OAuth2 exists in Innovapptive's reference architecture, but it is configured in\n    the CUSTOMER's SAP BTP tenant.\
  \ Innovapptive does not operate a public\n    authorization server, and no /.well-known/oauth-authorization-server or\n    /.well-known/openid-configuration was found on any Innovapptive host.\nspec_discovery:\n  openapi: not-published-anonymously\n  probes:\n  - url: https://cbo.innovapptive.com/operatorroundsapi/external/api-docs/\n    status: 200\n    result: Swagger UI HTML shell (3106 bytes)\n  - url: https://cbo.innovapptive.com/operatorroundsapi/external/api-docs-json\n    status: 404\n  - url: https://cbo.innovapptive.com/operatorroundsapi/external/v3/api-docs\n    status: 404\n  - url: https://cbo.innovapptive.com/operatorroundsapi/external/api-docs/swagger-ui-init.js\n    status: 404\n    note: >-\n      The Swagger UI shell references ./swagger-ui-bundle.js,\n      ./swagger-ui-standalone-preset.js and ./swagger-ui-init.js, but the edge\n      returns nginx 404 for all three, so the console does not render for an\n      anonymous visitor and the embedded document cannot be read.\n\
  \  - url: https://cwpuat2.innovapptive.com/operatorroundsapi/external/api-docs/\n    status: 200\n    result: same Swagger UI HTML shell (the Request URL named in the docs)\nx-evidence:\n  fetched: '2026-08-04'\n  http_status: 200\n  urls:\n  - https://docs.innovapptive.com/2605/mRounds_configuration_guide/html/topics/api_using_overview.html\n  - https://docs.innovapptive.com/2605/mRounds_configuration_guide/html/topics/api_generate_key.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/innovapptive/refs/heads/main/authentication/innovapptive-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Connected Worker
- Industrial
- Enterprise Asset Management
- Maintenance
- Warehouse
- EHS
- SAP
- IBM Maximo
- Mobile
- Manufacturing
- Oil and Gas
- Field Service
---
