---
api_key_in: []
api_specs:
- filename: oracle-siebel-event-pubsub-asyncapi.yml
  format: yaml
  label: Oracle Siebel Event Pub/Sub API
  slug: oracle-siebel-event-pubsub-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/asyncapi/oracle-siebel-event-pubsub-asyncapi.yml
- filename: oracle-siebel-accounts-api-openapi.yml
  format: yaml
  label: Oracle Siebel Accounts API
  slug: oracle-siebel-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-accounts-api-openapi.yml
- filename: oracle-siebel-activities-api-openapi.yml
  format: yaml
  label: Oracle Siebel Activities API
  slug: oracle-siebel-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-activities-api-openapi.yml
- filename: oracle-siebel-business-services-api-openapi.yml
  format: yaml
  label: Oracle Siebel Business Services API
  slug: oracle-siebel-business-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-business-services-api-openapi.yml
- filename: oracle-siebel-contacts-api-openapi.yml
  format: yaml
  label: Oracle Siebel Contacts API
  slug: oracle-siebel-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-contacts-api-openapi.yml
- filename: oracle-siebel-metadata-api-openapi.yml
  format: yaml
  label: Oracle Siebel Metadata API
  slug: oracle-siebel-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-metadata-api-openapi.yml
- filename: oracle-siebel-opportunities-api-openapi.yml
  format: yaml
  label: Oracle Siebel Opportunities API
  slug: oracle-siebel-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-opportunities-api-openapi.yml
- filename: oracle-siebel-orders-api-openapi.yml
  format: yaml
  label: Oracle Siebel Orders API
  slug: oracle-siebel-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-orders-api-openapi.yml
- filename: oracle-siebel-products-api-openapi.yml
  format: yaml
  label: Oracle Siebel Products API
  slug: oracle-siebel-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-products-api-openapi.yml
- filename: oracle-siebel-repository-api-openapi.yml
  format: yaml
  label: Oracle Siebel Repository API
  slug: oracle-siebel-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-repository-api-openapi.yml
- filename: oracle-siebel-service-requests-api-openapi.yml
  format: yaml
  label: Oracle Siebel Service Requests API
  slug: oracle-siebel-service-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/openapi/oracle-siebel-service-requests-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Oracle Siebel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Siebel declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Oracle Siebel
provider_slug: oracle-siebel
scheme_count: 2
schemes:
- description: HTTP Basic authentication using Siebel CRM user credentials. Applies when the Authentication type configured in siebsrvr.properties is Basic or SSO. The authenticated Siebel user's position and responsibilities determine record visibility, so authorization is data-level rather than scope-level.
  header: 'Authorization: Basic <base64(user:password)>'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/*.yml
  - https://docs.oracle.com/cd/G30554_01/books/RestAPI/c-About-Supported-HTTP-Header-Fields--ti1009563.html
  type: http
- description: OAuth 2.0 bearer-token access. Applies when the Authentication type configured in siebsrvr.properties is OAuth.
  header: 'Authorization: Bearer <access_token>'
  name: oauth2
  prerequisite: The Siebel Object Manager must be configured for SSO when OAuth is enabled for authentication.
  role: resource-server
  scope_handling: '"If the token scope is used while retrieving the token, then the token scope must match the executed operation." Scope names are defined by the customer''s own OAuth provider — Siebel publishes no scope registry.'
  sources:
  - openapi/*.yml
  - https://docs.oracle.com/cd/G30562_01/books/Secur/c-Using-OAuth-with-REST-Inbound-Web-Services.html
  token_issuer: external
  type: oauth2
  validation:
    method: introspection
    rfc: RFC 7662
    statement: '"The Siebel application supports only the introspection method of validating incoming access tokens." Signature-based validation of JWTs is explicitly unavailable.'
    transport: The Siebel REST API layer contacts the OAuth server over a secure channel (HTTPS) to validate the received access token or obtain additional token information. The OAuth server's certificates must be installed in the environment hosting the Siebel REST API.
    workaround: If JWTs must be validated by signature, validation has to happen at an API gateway BEFORE the request reaches Siebel.
slug: oracle-siebel-authentication
source_filename: oracle-siebel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://docs.oracle.com/cd/G30562_01/books/Secur/c-Using-OAuth-with-REST-Inbound-Web-Services.html,\n  https://docs.oracle.com/cd/G30554_01/books/RestAPI/c-About-Supported-HTTP-Header-Fields--ti1009563.html,\n  https://docs.oracle.com/cd/F26413_26/books/Secur/single-sign-on-authentication.html,\n  https://docs.oracle.com/cd/F26413_26/books/Secur/index.html —\n  upgraded from the securityScheme baseline derived out of openapi/*.yml\ndocs: https://docs.oracle.com/cd/F26413_26/books/Secur/index.html\nprovider: Oracle Siebel\nproviderId: oracle-siebel\nsummary: >-\n  Siebel REST authentication is decided by ONE server-side setting: the\n  Authentication type in siebsrvr.properties. Set it to Basic or SSO and callers\n  send `Authorization: Basic`; set it to OAuth and callers send `Authorization:\n  Bearer`. There is no per-client choice, and there is no API key. Siebel is a\n  resource server only — it never issues a token.\
  \ Bearer tokens come from an\n  external OAuth provider and are validated by INTROSPECTION over HTTPS on every\n  call.\nsummary_types:\n  types:\n    - http\n    - oauth2\n  oauth2_flows:\n    - external\n  api_keys: false\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    header: 'Authorization: Basic <base64(user:password)>'\n    description: >-\n      HTTP Basic authentication using Siebel CRM user credentials. Applies when\n      the Authentication type configured in siebsrvr.properties is Basic or SSO.\n      The authenticated Siebel user's position and responsibilities determine\n      record visibility, so authorization is data-level rather than scope-level.\n    sources:\n      - openapi/*.yml\n      - https://docs.oracle.com/cd/G30554_01/books/RestAPI/c-About-Supported-HTTP-Header-Fields--ti1009563.html\n  - name: oauth2\n    type: oauth2\n    header: 'Authorization: Bearer <access_token>'\n    role: resource-server\n    description: >-\n      OAuth 2.0 bearer-token\
  \ access. Applies when the Authentication type\n      configured in siebsrvr.properties is OAuth.\n    token_issuer: external\n    validation:\n      method: introspection\n      rfc: RFC 7662\n      statement: >-\n        \"The Siebel application supports only the introspection method of\n        validating incoming access tokens.\" Signature-based validation of JWTs is\n        explicitly unavailable.\n      transport: >-\n        The Siebel REST API layer contacts the OAuth server over a secure channel\n        (HTTPS) to validate the received access token or obtain additional token\n        information. The OAuth server's certificates must be installed in the\n        environment hosting the Siebel REST API.\n      workaround: >-\n        If JWTs must be validated by signature, validation has to happen at an\n        API gateway BEFORE the request reaches Siebel.\n    scope_handling: >-\n      \"If the token scope is used while retrieving the token, then the token\n      scope must\
  \ match the executed operation.\" Scope names are defined by the\n      customer's own OAuth provider — Siebel publishes no scope registry.\n    prerequisite: >-\n      The Siebel Object Manager must be configured for SSO when OAuth is enabled\n      for authentication.\n    sources:\n      - openapi/*.yml\n      - https://docs.oracle.com/cd/G30562_01/books/Secur/c-Using-OAuth-with-REST-Inbound-Web-Services.html\nconfiguration:\n  file: siebsrvr.properties\n  parameter: Authentication type\n  values:\n    - Basic\n    - SSO\n    - OAuth\n  note: >-\n    Server-wide. A single Siebel Application Interface cannot offer Basic to one\n    caller and Bearer to another.\nauthorization_model:\n  style: data-visibility\n  mechanism: >-\n    Siebel authorizes by Siebel responsibilities, positions and organization\n    visibility, applied per Business Component and modulated at call time by the\n    ViewMode query parameter. There are no API permissions, no roles exposed over\n    REST, and no scope-to-operation\
  \ mapping.\n  see_also: scopes/oracle-siebel-scopes.yml\nspec_discrepancy:\n  finding: >-\n    The OpenAPI documents in openapi/ declare an oauth2 authorizationCode flow\n    with authorizationUrl https://{siebel-server}/siebel/v1.0/auth/authorize and\n    tokenUrl https://{siebel-server}/siebel/v1.0/auth/token. Oracle documents no\n    such endpoints. Siebel does not host an authorization server; it validates\n    tokens issued elsewhere. Those two URLs should be read as spec-authoring\n    placeholders, not as callable endpoints.\n  action: >-\n    Recorded here and in overlays/ rather than silently propagated. Nothing in\n    this artifact is derived from those two URLs.\nmcp_authentication:\n  runtime: Siebel AI Connectors\n  scheme: oauth2-jwt\n  note: >-\n    The MCP runtime validates JWTs LOCALLY against a configured issuer,\n    audience, required scope and JWKS URI — the opposite of the Siebel REST\n    layer, which cannot do signature validation. See mcp/oracle-siebel-mcp.yml.\n\
  maintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-siebel/refs/heads/main/authentication/oracle-siebel-authentication.yml
summary_line: 2 schemes
tags:
- CRM
- Customer Management
- Enterprise Software
- Marketing Automation
- Oracle
- Sales Automation
- Service Automation
---
