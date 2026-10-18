---
api_specs:
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Products API
  slug: nacelle-storefront-products-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Product Collections API
  slug: nacelle-storefront-product-collections-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Content API
  slug: nacelle-storefront-content-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Storefront Navigation and Spaces API
  slug: nacelle-storefront-navigation-spaces-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle.postman_collection.json
  format: json
  label: Nacelle Admin Indexing and Ingestion API
  slug: nacelle-admin-indexing-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/collections/nacelle.postman_collection.json
- filename: nacelle-addresses-api-openapi.yml
  format: yaml
  label: Nacelle Addresses API
  slug: nacelle-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-addresses-api-openapi.yml
- filename: nacelle-checkout-api-openapi.yml
  format: yaml
  label: Nacelle Checkout API
  slug: nacelle-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-checkout-api-openapi.yml
- filename: nacelle-credentials-api-openapi.yml
  format: yaml
  label: Nacelle Credentials API
  slug: nacelle-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-credentials-api-openapi.yml
- filename: nacelle-customers-api-openapi.yml
  format: yaml
  label: Nacelle Customers API
  slug: nacelle-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-customers-api-openapi.yml
- filename: nacelle-entries-alpha-api-openapi.yml
  format: yaml
  label: Nacelle entries (ALPHA) API
  slug: nacelle-entries-alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-entries-alpha-api-openapi.yml
- filename: nacelle-entries-api-openapi.yml
  format: yaml
  label: Nacelle Entries API
  slug: nacelle-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-entries-api-openapi.yml
- filename: nacelle-entries-beta-api-openapi.yml
  format: yaml
  label: Nacelle entries (BETA) API
  slug: nacelle-entries-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-entries-beta-api-openapi.yml
- filename: nacelle-fulfillments-api-openapi.yml
  format: yaml
  label: Nacelle Fulfillments API
  slug: nacelle-fulfillments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-fulfillments-api-openapi.yml
- filename: nacelle-index-api-openapi.yml
  format: yaml
  label: Nacelle Index API
  slug: nacelle-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-index-api-openapi.yml
- filename: nacelle-multiorders-api-openapi.yml
  format: yaml
  label: Nacelle Multiorders API
  slug: nacelle-multiorders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-multiorders-api-openapi.yml
- filename: nacelle-orderitems-api-openapi.yml
  format: yaml
  label: Nacelle Orderitems API
  slug: nacelle-orderitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-orderitems-api-openapi.yml
- filename: nacelle-payment-api-openapi.yml
  format: yaml
  label: Nacelle Payment API
  slug: nacelle-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-payment-api-openapi.yml
- filename: nacelle-paymentintent-api-openapi.yml
  format: yaml
  label: Nacelle Paymentintent API
  slug: nacelle-paymentintent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-paymentintent-api-openapi.yml
- filename: nacelle-token-api-openapi.yml
  format: yaml
  label: Nacelle Token API
  slug: nacelle-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/openapi/nacelle-token-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: false
  dnssec: false
  domain: nacelle.com
  spf: true
hosts:
- cert_expires: Sep 13 19:15:48 2026 GMT
  host: nacelle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 14:01:32 2026 GMT
  host: docs.nacelle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: storefront.api.nacelle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Nacelle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nacelle, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Nacelle
provider_slug: nacelle
slug: nacelle-domain-security
source_filename: nacelle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nacelle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 19:15:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.nacelle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:01:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: storefront.api.nacelle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nacelle.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nacelle/refs/heads/main/security/nacelle-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Commerce
- Headless Commerce
- Composable Commerce
- GraphQL
- Content
- Data Indexing
---
