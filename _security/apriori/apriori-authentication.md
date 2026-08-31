---
api_key_in:
- header
- query
api_specs:
- filename: apriori-agent-api-openapi.yml
  format: yaml
  label: aPriori Agent API
  slug: apriori-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apriori/refs/heads/main/openapi/apriori-agent-api-openapi.yml
- filename: apriori-workflow-api-openapi.yml
  format: yaml
  label: aPriori Workflow API
  slug: apriori-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apriori/refs/heads/main/openapi/apriori-workflow-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Apriori Authentication
name_suffix: Authentication
oauth_flows: []
overview: aPriori secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: aPriori
provider_slug: apriori
scheme_count: 2
schemes:
- applies_to: all 12 operations
  description: Published by aPriori as security scheme "JWT Bearer" — type apiKey, name Authorization, in HEADER. Note that aPriori declares this as an apiKey scheme rather than as HTTP bearer, so no bearerFormat is published and no token endpoint, issuer or expiry policy is documented.
  in: header
  label: JWT Bearer
  name: JWTBearer
  parameter: Authorization
  sources:
  - openapi/apriori-ap-connect-agent.yml
  - https://docs.apriori.com/en/Connect/apc/rarg/Security/
  type: apiKey
- applies_to: all 12 operations
  description: Published by aPriori as security scheme "Shared Secret" — type apiKey, name key, in QUERY.
  in: query
  label: Shared Secret
  name: SharedSecret
  parameter: key
  risk: A credential carried in the query string is written to proxy, load-balancer and web-server access logs and can leak via Referer headers. Prefer the JWT Bearer header where the deployment allows it.
  sources:
  - openapi/apriori-ap-connect-agent.yml
  - https://docs.apriori.com/en/Connect/apc/rarg/Security/
  type: apiKey
slug: apriori-authentication
source_filename: apriori-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: openapi/apriori-ap-connect-agent.yml\ndocs:\n- https://docs.apriori.com/en/Connect/apc/rarg/Security/\n- https://docs.apriori.com/en/Connect/apc/sag/REST-API-Management-Responsibilities/\n- https://docs.apriori.com/en/Connect/apc/rn/release-notes/\n- https://www.apriori.com/security/\napi: aP Connect Agent REST API\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\n  oauth2: false\n  openid_connect: false\n  mutual_tls: true\n  mutual_tls_scope: transport, configured on the Connector — not selectable per request\nschemes:\n- name: JWTBearer\n  label: JWT Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Published by aPriori as security scheme \"JWT Bearer\" — type apiKey, name Authorization, in HEADER.\n    Note that aPriori declares this as an apiKey scheme rather than as HTTP bearer, so no bearerFormat is\n    published and no token endpoint, issuer or expiry policy\
  \ is documented.\n  applies_to: all 12 operations\n  sources:\n  - openapi/apriori-ap-connect-agent.yml\n  - https://docs.apriori.com/en/Connect/apc/rarg/Security/\n- name: SharedSecret\n  label: Shared Secret\n  type: apiKey\n  in: query\n  parameter: key\n  description: >-\n    Published by aPriori as security scheme \"Shared Secret\" — type apiKey, name key, in QUERY.\n  applies_to: all 12 operations\n  risk: >-\n    A credential carried in the query string is written to proxy, load-balancer and web-server access logs\n    and can leak via Referer headers. Prefer the JWT Bearer header where the deployment allows it.\n  sources:\n  - openapi/apriori-ap-connect-agent.yml\n  - https://docs.apriori.com/en/Connect/apc/rarg/Security/\ntransport_security:\n  mtls:\n    supported: true\n    since: '2026-06-30'\n    requires: aP Connect Agent 5.2.0 or later\n    configuration: >-\n      Enable the mTLS option when creating the Connector, then supply the aPriori-signed certificate during\n  \
  \    Agent installation. The certificate must be obtained from aPriori Support before install.\n    install_modes:\n      supported: [Setup Wizard, console (-c)]\n      unsupported: [unattended (-q)]\n    replaces: IP allowlisting of the Agent host\n    rationale_published: >-\n      \"This is increasingly important for organizations who may be unable to guarantee static IP addresses.\"\n    source: https://docs.apriori.com/en/Connect/apc/rn/release-notes/\n  certificates:\n    jdk_import_required: true\n    note: >-\n      aPriori documents importing Java Developer Kit certificates and obtaining a signed certificate as part\n      of Agent installation.\n    source: https://docs.apriori.com/en/Connect/apc/ig/Importing-Java-Developer-Kit-Certificates/\napplication_sso:\n  scope: aPriori Cloud application sign-in — NOT the API\n  provider: Auth0\n  detail: >-\n    aPriori's security page states that single sign-on runs through a dedicated Auth0 production tenant with\n    SAML integration\
  \ to customer identity providers. This governs human login to aPriori Cloud\n    (https://cloud.apriori.net/), not machine access to the Agent API.\n  source: https://www.apriori.com/security/\n  instructions: https://www.apriori.com/sso-instructions-page/\nnot_published:\n- No OAuth 2.0 flow, authorization server, token endpoint or scope model for the API.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any host (probed; see well-known/apriori-well-known.yml).\n- No key rotation, expiry or revocation policy for the JWT or the shared secret.\n- No self-serve credential issuance. Access to the API follows a paid deployment; aPriori recommends an aPriori System Services engagement for leveraging it on a file-system deployment.\nx-evidence:\n  fetched: '2026-08-06'\n  sources:\n  - url: https://docs.apriori.com/en/Connect/apc/rarg/Security/\n    http_status: 200\n  - url: https://docs.apriori.com/en/Connect/apc/sag/REST-API-Management-Responsibilities/\n\
  \    http_status: 200\n  - url: https://docs.apriori.com/en/Connect/apc/rn/release-notes/\n    http_status: 200\n  - url: https://www.apriori.com/security/\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apriori/refs/heads/main/authentication/apriori-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Manufacturing
- product-cost-management
- design-for-manufacturability
- should-cost
- plm-integration
- cost-engineering
- digital-manufacturing
- sustainability
- workflow-automation
- cad
---
