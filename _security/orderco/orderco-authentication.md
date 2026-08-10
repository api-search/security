---
api_key_in: []
api_specs:
- filename: orderco-components-api-openapi.yml
  format: yaml
  label: Order.co Components API
  slug: orderco-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-components-api-openapi.yml
- filename: orderco-content-api-openapi.yml
  format: yaml
  label: Order.co Content API
  slug: orderco-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-content-api-openapi.yml
- filename: orderco-customer-stories-api-openapi.yml
  format: yaml
  label: Order.co Customer Stories API
  slug: orderco-customer-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-customer-stories-api-openapi.yml
- filename: orderco-discovery-api-openapi.yml
  format: yaml
  label: Order.co Discovery API
  slug: orderco-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-discovery-api-openapi.yml
- filename: orderco-faqs-api-openapi.yml
  format: yaml
  label: Order.co FA Qs API
  slug: orderco-faqs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-faqs-api-openapi.yml
- filename: orderco-incidents-api-openapi.yml
  format: yaml
  label: Order.co Incidents API
  slug: orderco-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-incidents-api-openapi.yml
- filename: orderco-maintenance-api-openapi.yml
  format: yaml
  label: Order.co Maintenance API
  slug: orderco-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-maintenance-api-openapi.yml
- filename: orderco-newsroom-api-openapi.yml
  format: yaml
  label: Order.co Newsroom API
  slug: orderco-newsroom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-newsroom-api-openapi.yml
- filename: orderco-resources-api-openapi.yml
  format: yaml
  label: Order.co Resources API
  slug: orderco-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-resources-api-openapi.yml
- filename: orderco-search-api-openapi.yml
  format: yaml
  label: Order.co Search API
  slug: orderco-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-search-api-openapi.yml
- filename: orderco-status-api-openapi.yml
  format: yaml
  label: Order.co Status API
  slug: orderco-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-status-api-openapi.yml
- filename: orderco-taxonomies-api-openapi.yml
  format: yaml
  label: Order.co Taxonomies API
  slug: orderco-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-taxonomies-api-openapi.yml
- filename: orderco-testimonials-api-openapi.yml
  format: yaml
  label: Order.co Testimonials API
  slug: orderco-testimonials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-testimonials-api-openapi.yml
- filename: orderco-vendor-stories-api-openapi.yml
  format: yaml
  label: Order.co Vendor Stories API
  slug: orderco-vendor-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/openapi/orderco-vendor-stories-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Orderco Authentication
name_suffix: Authentication
oauth_flows: []
overview: Order.co declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Order.co
provider_slug: orderco
scheme_count: 0
schemes: []
slug: orderco-authentication
source_filename: orderco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: >-\n  Derived from openapi/orderco-content-openapi.yml and openapi/orderco-status-openapi.yml, plus\n  the authentication block of the WordPress REST discovery document at\n  https://www.order.co/wp-json/ and live anonymous probes on 2026-08-04.\nsummary: >-\n  Neither public Order.co surface requires authentication, because neither is the product. Every\n  operation in both generated OpenAPIs is an anonymous GET. The product API - the one Order.co\n  markets to accounting and ERP buyers, and the one whose credentials vendors receive at\n  onboarding - has no publicly documented authentication scheme at all: no OAuth metadata, no\n  OpenID configuration, no API-key documentation, no /.well-known/ document on any Order.co host.\nsurfaces:\n- key: content\n  name: Order.co Content API\n  base_url: https://www.order.co/wp-json\n  openapi: openapi/orderco-content-openapi.yml\n  security_schemes: []\n  anonymous_read: true\n  note:\
  \ >-\n    All 37 modelled operations are anonymous GETs. The discovery document advertises exactly one\n    authentication mechanism - WordPress Application Passwords (HTTP Basic), authorization\n    endpoint https://www.order.co/wp-admin/authorize-application.php. That is a site-administration\n    credential for the marketing CMS, not a developer program, and it is recorded here only so the\n    profile is complete. Write routes and the administrative namespaces return\n    HTTP 401 `rest_forbidden` anonymously (verified against /wp/v2/users and\n    /wp-abilities/v1/abilities).\n  advertised_scheme:\n    type: http\n    scheme: basic\n    name: WordPress Application Passwords\n    authorization_endpoint: https://www.order.co/wp-admin/authorize-application.php\n    first_party_developer_program: false\n- key: status\n  name: Order.co Status API\n  base_url: https://status.order.co/api/v2\n  openapi: openapi/orderco-status-openapi.yml\n  security_schemes: []\n  anonymous_read: true\n\
  \  note: >-\n    All eight Statuspage v2 endpoints returned HTTP 200 without credentials. Responses carry\n    `access-control-allow-origin: *`, so they are callable from a browser.\nproduct_api:\n  documented: false\n  reference_url: null\n  auth_scheme: undisclosed\n  evidence:\n  - url: https://www.order.co/accounting-integrations/\n    status: 200\n    quote: Order.co seamlessly connects to your accounting system via API - it's as simple as 1, 2, 3.\n  - url: https://developer.order.co/\n    status: 200\n    note: Wildcard DNS; resolves to the marketing site, not a developer portal.\n  - url: https://api.order.co/openapi.json\n    status: 404\n  - url: https://app.order.co/login\n    status: 200\n    note: The customer application sign-in page. Everything past it is credentialed.\n  note: >-\n    Order.co names QuickBooks Online, NetSuite, Sage Intacct and Workday as API integrations, and\n    its own vendor-onboarding material describes portal account creation plus API or EDI\n  \
  \  credentials. None of that surface is publicly documented, so no authentication profile can be\n    recorded for it without inventing one.\nwell_known:\n  openid_configuration: absent\n  oauth_authorization_server: absent\n  oauth_protected_resource: absent\n  probed: well-known/orderco-well-known.yml\nsso_for_the_product:\n  documented: true\n  url: https://www.order.co/sso-integrations/\n  providers:\n  - Okta\n  - Ping Identity\n  note: >-\n    Single sign-on into the Order.co application for end users. Not API authentication, and not\n    an OIDC surface a developer can discover - no issuer, no discovery document is published.\nprovider_gaps:\n- Publish the authentication scheme for the customer API (key, OAuth 2.0 client credentials, or\n  otherwise) at a public URL.\n- If OAuth 2.0 or OIDC is in use, serve /.well-known/oauth-authorization-server or\n  /.well-known/openid-configuration so the surface is machine-discoverable.\n- Publish the vendor API credential model instead of\
  \ disclosing it only during onboarding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orderco/refs/heads/main/authentication/orderco-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Procurement
- Spend Management
- Accounts Payable
- Purchasing
- Vendor Management
- Payments
- Virtual Cards
- Finance Automation
- United States
---
