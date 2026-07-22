---
api_specs:
- filename: skimbit-merchant-openapi.yml
  format: yaml
  label: Skimlinks Merchant API
  slug: skimlinks-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-merchant-openapi.yml
- filename: skimbit-reporting-openapi.yml
  format: yaml
  label: Skimlinks Reporting API
  slug: skimlinks-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-reporting-openapi.yml
- filename: skimbit-product-key-openapi.yml
  format: yaml
  label: Skimlinks Product Key API
  slug: skimlinks-product-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimbit/refs/heads/main/openapi/skimbit-product-key-openapi.yml
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
- cert_expires: Sep  2 10:05:29 2026 GMT
  host: developers.skimlinks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 20:53:38 2026 GMT
  host: merchants.skimapis.com
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
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skimlinks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: developers.skimlinks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 10:05:29 2026 GMT\n  hsts: false\n- host: merchants.skimapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 20:53:38 2026 GMT\n  hsts: null\ndomains:\n- domain: skimlinks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: skimapis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
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
