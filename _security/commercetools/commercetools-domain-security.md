---
api_specs:
- filename: commercetools-carts-api-openapi.yml
  format: yaml
  label: commercetools Carts API
  slug: commercetools-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-carts-api-openapi.yml
- filename: commercetools-categories-api-openapi.yml
  format: yaml
  label: commercetools Categories API
  slug: commercetools-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-categories-api-openapi.yml
- filename: commercetools-changehistory-api-openapi.yml
  format: yaml
  label: commercetools ChangeHistory API
  slug: commercetools-changehistory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-changehistory-api-openapi.yml
- filename: commercetools-customers-api-openapi.yml
  format: yaml
  label: commercetools Customers API
  slug: commercetools-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-customers-api-openapi.yml
- filename: commercetools-importcontainers-api-openapi.yml
  format: yaml
  label: commercetools ImportContainers API
  slug: commercetools-importcontainers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-importcontainers-api-openapi.yml
- filename: commercetools-importoperations-api-openapi.yml
  format: yaml
  label: commercetools ImportOperations API
  slug: commercetools-importoperations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-importoperations-api-openapi.yml
- filename: commercetools-inventory-api-openapi.yml
  format: yaml
  label: commercetools Inventory API
  slug: commercetools-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-inventory-api-openapi.yml
- filename: commercetools-orders-api-openapi.yml
  format: yaml
  label: commercetools Orders API
  slug: commercetools-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-orders-api-openapi.yml
- filename: commercetools-payments-api-openapi.yml
  format: yaml
  label: commercetools Payments API
  slug: commercetools-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-payments-api-openapi.yml
- filename: commercetools-products-api-openapi.yml
  format: yaml
  label: commercetools Products API
  slug: commercetools-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-products-api-openapi.yml
- filename: commercetools-productvariants-api-openapi.yml
  format: yaml
  label: commercetools ProductVariants API
  slug: commercetools-productvariants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-productvariants-api-openapi.yml
- filename: commercetools-project-api-openapi.yml
  format: yaml
  label: commercetools Project API
  slug: commercetools-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-project-api-openapi.yml
- filename: commercetools-standaloneprices-api-openapi.yml
  format: yaml
  label: commercetools StandalonePrices API
  slug: commercetools-standaloneprices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-standaloneprices-api-openapi.yml
- filename: commercetools-subscriptions-api-openapi.yml
  format: yaml
  label: commercetools Subscriptions API
  slug: commercetools-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/openapi/commercetools-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "rapidssl.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: commercetools.com
  spf: true
hosts:
- cert_expires: Sep 12 12:45:08 2026 GMT
  host: commercetools.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 10:16:07 2026 GMT
  host: docs.commercetools.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Commercetools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for commercetools, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: commercetools
provider_slug: commercetools
slug: commercetools-domain-security
source_filename: commercetools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: commercetools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 12:45:08 2026 GMT\n  hsts: false\n- host: docs.commercetools.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 10:16:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: commercetools.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"rapidssl.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commercetools/refs/heads/main/security/commercetools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commerce
- Composable Commerce
- E-Commerce
- GraphQL
- REST
- SDK
---
