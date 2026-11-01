---
api_specs:
- filename: bol-com-commissions-api-openapi.yml
  format: yaml
  label: Bol Commissions API
  slug: bol-com-commissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-commissions-api-openapi.yml
- filename: bol-com-insights-api-openapi.yml
  format: yaml
  label: Bol Insights API
  slug: bol-com-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-insights-api-openapi.yml
- filename: bol-com-inventory-api-openapi.yml
  format: yaml
  label: Bol Inventory API
  slug: bol-com-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-inventory-api-openapi.yml
- filename: bol-com-invoices-api-openapi.yml
  format: yaml
  label: Bol Invoices API
  slug: bol-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-invoices-api-openapi.yml
- filename: bol-com-offers-api-openapi.yml
  format: yaml
  label: Bol Offers API
  slug: bol-com-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-offers-api-openapi.yml
- filename: bol-com-orders-api-openapi.yml
  format: yaml
  label: Bol Orders API
  slug: bol-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-orders-api-openapi.yml
- filename: bol-com-products-api-openapi.yml
  format: yaml
  label: Bol Products API
  slug: bol-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-products-api-openapi.yml
- filename: bol-com-promotions-api-openapi.yml
  format: yaml
  label: Bol Promotions API
  slug: bol-com-promotions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-promotions-api-openapi.yml
- filename: bol-com-replenishments-api-openapi.yml
  format: yaml
  label: Bol Replenishments API
  slug: bol-com-replenishments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-replenishments-api-openapi.yml
- filename: bol-com-retailers-api-openapi.yml
  format: yaml
  label: Bol Retailers API
  slug: bol-com-retailers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-retailers-api-openapi.yml
- filename: bol-com-returns-api-openapi.yml
  format: yaml
  label: Bol Returns API
  slug: bol-com-returns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-returns-api-openapi.yml
- filename: bol-com-shipments-api-openapi.yml
  format: yaml
  label: Bol Shipments API
  slug: bol-com-shipments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-shipments-api-openapi.yml
- filename: bol-com-shipping-labels-api-openapi.yml
  format: yaml
  label: Bol Shipping Labels API
  slug: bol-com-shipping-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-shipping-labels-api-openapi.yml
- filename: bol-com-subscriptions-api-openapi.yml
  format: yaml
  label: Bol Subscriptions API
  slug: bol-com-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-subscriptions-api-openapi.yml
- filename: bol-com-transports-api-openapi.yml
  format: yaml
  label: Bol Transports API
  slug: bol-com-transports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bol-com/openapi/bol-com-transports-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "geotrust.com"
  - 0 issuewild "geotrust.com"
  - 0 issue "thawte.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:abuse@bol.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bol.com
  spf: true
hosts:
- cert_expires: Nov 28 09:56:27 2026 GMT
  host: bol.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bol Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bol
provider_slug: bol-com
slug: bol-com-domain-security
source_filename: bol-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 09:56:27 2026 GMT\n  hsts: null\ndomains:\n- domain: bol.com\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"geotrust.com\"\n  - 0 issuewild \"geotrust.com\"\n  - 0 issue \"thawte.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:abuse@bol.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bol-com/security/bol-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- e-commerce
- retail
- marketplace
- API
- Netherlands
---
