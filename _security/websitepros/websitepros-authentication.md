---
api_key_in:
- header
api_specs:
- filename: websitepros-domains-api-openapi.yml
  format: yaml
  label: WebsitePros Domains API
  slug: websitepros-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/openapi/websitepros-domains-api-openapi.yml
- filename: websitepros-health-api-openapi.yml
  format: yaml
  label: WebsitePros Health API
  slug: websitepros-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/openapi/websitepros-health-api-openapi.yml
- filename: websitepros-sales-orders-api-openapi.yml
  format: yaml
  label: WebsitePros Sales Orders API
  slug: websitepros-sales-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/openapi/websitepros-sales-orders-api-openapi.yml
- filename: websitepros-service-orders-api-openapi.yml
  format: yaml
  label: WebsitePros Service Orders API
  slug: websitepros-service-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/openapi/websitepros-service-orders-api-openapi.yml
- filename: websitepros-sso-api-openapi.yml
  format: yaml
  label: WebsitePros SSO API
  slug: websitepros-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/openapi/websitepros-sso-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Websitepros Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: WebsitePros secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: WebsitePros
provider_slug: websitepros
scheme_count: 5
schemes:
- description: Azure API Management subscription key identifying your subscription to the API. Issued separately per environment after Web.com International manually reviews and approves your developer-portal registration.
  evidence:
    http_status: 401
    url: https://api.nts.web.com/sales-orders/v1
    www_authenticate: AzureApiManagementKey realm="https://api.nts.web.com/sales-orders",name="Ocp-Apim-Subscription-Key",type="header"
  in: header
  name: subscriptionKey
  parameter: Ocp-Apim-Subscription-Key
  required: true
  type: apiKey
- description: 'Access token from the Web.com Microsoft Entra ID tenant, sent as `Authorization: Bearer`. The published collection obtains it with the client-credentials grant.'
  name: bearerAuth
  required: true
  scheme: bearer
  type: http
- applies_to:
  - createSalesOrder
  - listSalesOrders
  - getSalesOrderById
  - updateSalesOrder
  - deleteSalesOrder
  description: Your company's unique identifier, supplied by Web.com when the subscription is activated. Required on the sales-order operations.
  in: header
  name: tenantId
  parameter: x-nts-tenant-id
  required: true
  type: apiKey
- applies_to:
  - checkDomainAvailability
  - spinDomainSuggestions
  - getCustomerSsoUrl
  - createServiceOrders
  description: Your tenant's name, used in place of x-nts-tenant-id on the domain, SSO and service-order operations.
  in: header
  name: tenantName
  parameter: tenant-name
  required: true
  type: apiKey
- flows:
  - audience: api://intl.web.com
    content_type: application/x-www-form-urlencoded
    flow: clientCredentials
    parameters:
    - grant_type
    - client_id
    - client_secret
    - resource
    scopes: {}
    scopes_note: Web.com publishes no scope list. The v1 Entra endpoint in the published collection takes a `resource` audience (api://intl.web.com) rather than scopes, so there is no scope surface to record and no scopes/ artifact in this repository.
    tokenUrl: https://login.microsoftonline.com/03fbebc8-de8a-4428-b573-4c4903610dac/oauth2/token
  identity_provider:
    discovery: https://login.microsoftonline.com/03fbebc8-de8a-4428-b573-4c4903610dac/v2.0/.well-known/openid-configuration
    discovery_status: 200
    issuer: https://login.microsoftonline.com/03fbebc8-de8a-4428-b573-4c4903610dac/v2.0
    name: Microsoft Entra ID (Azure AD)
    note: The OIDC discovery document is served by Microsoft, not by Web.com. It is recorded here as the token authority for this API; it is NOT counted as a Web.com-served /.well-known surface, and no WellKnown pointer is emitted for it.
    tenant_id: 03fbebc8-de8a-4428-b573-4c4903610dac
  name: oauth2ClientCredentials
  type: oauth2
slug: websitepros-authentication
source_filename: websitepros-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api-docs.intl.web.com/\ndocs: https://api-docs.intl.web.com/\nnote: >-\n  Read from Web.com's own published \"International Platform Documentation\" (the public Postman\n  collection at api-docs.intl.web.com) and confirmed against live challenges observed on\n  api.nts.web.com on 2026-08-13. Web.com publishes no OpenAPI, so the scheme list below is\n  documentary, not spec-derived; it is mirrored into the derived spec at\n  openapi/websitepros-international-platform-openapi-derived.yml.\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  layered: true\n  layered_note: >-\n    Three credentials travel on the same request: an Azure API Management subscription key, a\n    Microsoft Entra ID bearer token, and a tenant identifier. None of the three is sufficient on\n    its own.\nschemes:\n  - name: subscriptionKey\n    type: apiKey\n    in: header\n    parameter: Ocp-Apim-Subscription-Key\n\
  \    description: >-\n      Azure API Management subscription key identifying your subscription to the API. Issued\n      separately per environment after Web.com International manually reviews and approves your\n      developer-portal registration.\n    required: true\n    evidence:\n      url: https://api.nts.web.com/sales-orders/v1\n      http_status: 401\n      www_authenticate: >-\n        AzureApiManagementKey realm=\"https://api.nts.web.com/sales-orders\",name=\"Ocp-Apim-Subscription-Key\",type=\"header\"\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Access token from the Web.com Microsoft Entra ID tenant, sent as `Authorization: Bearer`.\n      The published collection obtains it with the client-credentials grant.\n    required: true\n  - name: tenantId\n    type: apiKey\n    in: header\n    parameter: x-nts-tenant-id\n    description: >-\n      Your company's unique identifier, supplied by Web.com when the subscription is activated.\n  \
  \    Required on the sales-order operations.\n    required: true\n    applies_to: [createSalesOrder, listSalesOrders, getSalesOrderById, updateSalesOrder, deleteSalesOrder]\n  - name: tenantName\n    type: apiKey\n    in: header\n    parameter: tenant-name\n    description: >-\n      Your tenant's name, used in place of x-nts-tenant-id on the domain, SSO and service-order\n      operations.\n    required: true\n    applies_to: [checkDomainAvailability, spinDomainSuggestions, getCustomerSsoUrl, createServiceOrders]\n  - name: oauth2ClientCredentials\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://login.microsoftonline.com/03fbebc8-de8a-4428-b573-4c4903610dac/oauth2/token\n        audience: api://intl.web.com\n        parameters: [grant_type, client_id, client_secret, resource]\n        content_type: application/x-www-form-urlencoded\n        scopes: {}\n        scopes_note: >-\n          Web.com publishes no scope list. The v1 Entra endpoint in\
  \ the published collection takes a\n          `resource` audience (api://intl.web.com) rather than scopes, so there is no scope surface\n          to record and no scopes/ artifact in this repository.\n    identity_provider:\n      name: Microsoft Entra ID (Azure AD)\n      tenant_id: 03fbebc8-de8a-4428-b573-4c4903610dac\n      discovery: https://login.microsoftonline.com/03fbebc8-de8a-4428-b573-4c4903610dac/v2.0/.well-known/openid-configuration\n      discovery_status: 200\n      issuer: https://login.microsoftonline.com/03fbebc8-de8a-4428-b573-4c4903610dac/v2.0\n      note: >-\n        The OIDC discovery document is served by Microsoft, not by Web.com. It is recorded here as\n        the token authority for this API; it is NOT counted as a Web.com-served /.well-known\n        surface, and no WellKnown pointer is emitted for it.\nonboarding:\n  model: request-access\n  steps:\n    - Register at the developer portal for the environment you want (production and development are separate\
  \ registrations).\n    - Verify your email address from the link Web.com sends.\n    - Wait for Web.com International to review and activate your subscription; they also issue your Tenant Id.\n    - Retrieve your subscription keys from the developer portal.\n    - Call the healthcheck operation to confirm connectivity.\n  portals:\n    - environment: production\n      portal: https://nts.developer.azure-api.net\n      gateway: https://api.nts.web.com\n      portal_status: 200\n    - environment: development\n      portal: https://ntsdev.developer.azure-api.net\n      gateway: https://api-dev.nts.web.com\n      portal_status: 200\ngaps:\n  - >-\n    The developer portal's anonymous API list is empty (GET\n    https://nts.developer.azure-api.net/developer/apis?api-version=2022-04-01-preview returned\n    200 with {\"value\":[],\"nextLink\":null}), so the Azure API Management OpenAPI export that would\n    normally back this API is visible only to approved, signed-in subscribers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/websitepros/refs/heads/main/authentication/websitepros-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Company
- Website Builder
- Web Hosting
- Domains
- Small Business
- Digital Marketing
- E-Commerce
- Reseller
- Sales Orders
- Provisioning
- Single Sign-On
- Azure API Management
---
