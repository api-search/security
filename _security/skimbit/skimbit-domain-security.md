---
api_specs:
- filename: skimbit-commissions-api-openapi.yml
  format: yaml
  label: SkimBit Commissions API
  slug: skimbit-commissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-commissions-api-openapi.yml
- filename: skimbit-domains-api-openapi.yml
  format: yaml
  label: SkimBit Domains API
  slug: skimbit-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-domains-api-openapi.yml
- filename: skimbit-merchants-api-openapi.yml
  format: yaml
  label: SkimBit Merchants API
  slug: skimbit-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-merchants-api-openapi.yml
- filename: skimbit-offers-api-openapi.yml
  format: yaml
  label: SkimBit Offers API
  slug: skimbit-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-offers-api-openapi.yml
- filename: skimbit-payments-api-openapi.yml
  format: yaml
  label: SkimBit Payments API
  slug: skimbit-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-payments-api-openapi.yml
- filename: skimbit-products-api-openapi.yml
  format: yaml
  label: SkimBit Products API
  slug: skimbit-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-products-api-openapi.yml
- filename: skimbit-reports-api-openapi.yml
  format: yaml
  label: SkimBit Reports API
  slug: skimbit-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-reports-api-openapi.yml
- filename: skimbit-verticals-api-openapi.yml
  format: yaml
  label: SkimBit Verticals API
  slug: skimbit-verticals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-verticals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: skimlinks.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: skimapis.com
  spf: false
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: skimlinks.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 11:32:06 2026 GMT
  host: developers.skimlinks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 20:53:38 2026 GMT
  host: reporting.skimapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skimbit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SkimBit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SkimBit
provider_slug: skimbit
slug: skimbit-domain-security
source_filename: skimbit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skimlinks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developers.skimlinks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 11:32:06 2026 GMT\n  hsts: false\n- host: reporting.skimapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 20:53:38 2026 GMT\n  hsts: null\ndomains:\n- domain: skimlinks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: skimapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/security/skimbit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Affiliate Marketing
- Content Monetization
- Commerce
- Publishers
- Advertising
- Retail
- Reporting
- Products
- eCommerce
---
