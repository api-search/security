---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: watchmaker-genomics-commerce-rest-swagger.json
  format: json
  label: Watchmaker Genomics Storefront REST API
  slug: watchmaker-genomics-storefront-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/watchmaker-genomics/refs/heads/main/openapi/watchmaker-genomics-commerce-rest-swagger.json
auth_types:
- apiKey
- http-bearer
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Watchmaker Genomics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Watchmaker Genomics secures its APIs with apiKey and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Watchmaker Genomics
provider_slug: watchmaker-genomics
scheme_count: 2
schemes:
- applied_to_operations: 0
  declared_in: openapi/watchmaker-genomics-commerce-rest-swagger.json
  in: header
  name: api_key
  note: The only scheme in securityDefinitions. It is declared at document level and applied to NONE of the 70 operations — there is no `security` block on any path — so the contract does not say which operations need it. That has to be discovered by calling them.
  parameter: api_key
  sources:
  - openapi/watchmaker-genomics-commerce-rest-swagger.json
  type: apiKey
- declared_in: null
  in: header
  name: bearer
  note: 'Magento integration tokens are accepted as `Authorization: Bearer <token>` as well as via the api_key header. Not declared in the published document; inferred from the token-issuance operations that ARE in it.'
  parameter: Authorization
  scheme: bearer
  type: http
slug: watchmaker-genomics-authentication
source_filename: watchmaker-genomics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  openapi/watchmaker-genomics-commerce-rest-swagger.json (derived), plus live anonymous and\n  unauthorized requests to https://www.watchmakergenomics.com/rest/... and\n  https://www.watchmakergenomics.com/graphql on 2026-09-04\nnote: >-\n  Watchmaker Genomics publishes no authentication documentation. This profile is the securityScheme\n  the self-served Swagger declares, corrected and extended by what the live host actually did. The\n  headline fact is that a large, useful slice of this API needs no credential at all, and the part\n  that does need one cannot be credentialed by a member of the public.\nsummary:\n  types:\n  - apiKey\n  - http-bearer\n  api_key_in:\n  - header\n  anonymous_surface: true\n  public_credential_obtainable: false\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: api_key\n  declared_in: openapi/watchmaker-genomics-commerce-rest-swagger.json\n  applied_to_operations: 0\n  note:\
  \ >-\n    The only scheme in securityDefinitions. It is declared at document level and applied to NONE\n    of the 70 operations — there is no `security` block on any path — so the contract does not say\n    which operations need it. That has to be discovered by calling them.\n  sources:\n  - openapi/watchmaker-genomics-commerce-rest-swagger.json\n- name: bearer\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  declared_in: null\n  note: >-\n    Magento integration tokens are accepted as `Authorization: Bearer <token>` as well as via the\n    api_key header. Not declared in the published document; inferred from the token-issuance\n    operations that ARE in it.\ntoken_issuance:\n- operationId: PostV1IntegrationAdminToken\n  path: /V1/integration/admin/token\n  method: POST\n  note: Admin token. Requires admin credentials, which are not publicly obtainable.\n- operationId: PostV1IntegrationCustomerToken\n  path: /V1/integration/customer/token\n  method: POST\n\
  \  note: >-\n    Customer token. Requires a customer account, and this storefront's registration and login\n    routes both return 404 (probed 2026-09-04).\n- field: generateCustomerToken\n  surface: graphql\n  note: The GraphQL equivalent. Same account precondition, same blocker.\nsurfaces:\n- surface: rest\n  endpoint: https://www.watchmakergenomics.com/rest/all\n  anonymous_operations: 'the guest slice — directory, guest carts, checkout estimation and placement, customer creation and password reset, gift cards, in-store pickup, search, Magefan blog'\n  evidence:\n    verified_anonymous:\n      url: https://www.watchmakergenomics.com/rest/V1/directory/currency\n      status: 200\n      body_excerpt: '{\"base_currency_code\":\"USD\",\"base_currency_symbol\":\"$\",...}'\n    verified_gated:\n      url: https://www.watchmakergenomics.com/rest/V1/store/storeConfigs\n      status: 401\n      body: '{\"message\":\"The consumer isn''t authorized to access %resources.\",\"parameters\":{\"resources\"\
  :\"Magento_Backend::store\"}}'\n      note: >-\n        The 401 body names the exact Magento ACL resource required. That is unusually useful for a\n        caller, and it is the only place the contract's access model is expressed at all — 401 is\n        declared on no operation in the Swagger.\n- surface: graphql\n  endpoint: https://www.watchmakergenomics.com/graphql\n  anonymous_operations: 'catalog, categories, search, CMS, route resolution, storeConfig, guest cart, checkout estimation, contactUs, newsletter subscription, introspection'\n  authenticated_operations: 'customer, customerCart, customerOrders, wishlists, gift registries, returns, reward points, store credit'\n  auth_header: 'Authorization: Bearer <customer token>'\n  evidence:\n    verified_anonymous:\n      url: https://www.watchmakergenomics.com/graphql\n      status: 200\n      note: >-\n        Full IntrospectionQuery returned a 636-type schema with no credential — introspection is\n        not disabled on this deployment.\n\
  - surface: soap\n  endpoint: https://www.watchmakergenomics.com/soap/all\n  anonymous_operations: 'none — contract retrieval only'\n  evidence:\n    verified_anonymous:\n      url: 'https://www.watchmakergenomics.com/soap/all?wsdl_list=1'\n      status: 200\n      note: 200 services enumerated without credentials. The WSDLs are public; invocation is not.\noauth:\n  supported: false\n  evidence:\n  - {url: 'https://www.watchmakergenomics.com/.well-known/oauth-authorization-server', status: 404}\n  - {url: 'https://www.watchmakergenomics.com/.well-known/openid-configuration', status: 404}\n  note: >-\n    No oauth2 or openIdConnect securityScheme is declared and no discovery document is served, so\n    no scopes/ artifact is written for this provider.\nmtls:\n  supported: false\ntransport_security:\n  https_required: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31557600\ncookies:\n  note: >-\n    The GraphQL endpoint sets PHPSESSID and private_content_version on anonymous\
  \ POSTs. They are\n    not required for any read operation; a stateless client should discard them.\ngaps:\n- 'No authentication documentation of any kind is published by Watchmaker Genomics.'\n- 'The declared api_key scheme is applied to zero operations, so the contract does not distinguish public from gated.'\n- '401 is returned but declared on no operation.'\n- 'No public path exists to obtain a credential — registration and login both 404.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watchmaker-genomics/refs/heads/main/authentication/watchmaker-genomics-authentication.yml
summary_line: apiKey/http-bearer · 2 schemes
tags:
- Genomics
- Life Sciences
- Next-Generation Sequencing
- Molecular Diagnostics
- Biotechnology
- Reagents
- Bioinformatics
- E-Commerce
- GraphQL
- Adobe Commerce
---
