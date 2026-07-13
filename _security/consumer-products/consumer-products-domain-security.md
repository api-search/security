---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Open Food Facts
  slug: open-food-facts
  spec_type: OpenAPI
  url: https://openfoodfacts.github.io/openfoodfacts-server/api/ref-v2/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gs1.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openfoodfacts.org
  spf: true
hosts:
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: www.gs1.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: ref.gs1.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 15:07:01 2026 GMT
  host: world.openfoodfacts.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Consumer Products Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Consumer Products, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Consumer Products
provider_slug: consumer-products
slug: consumer-products-domain-security
source_filename: consumer-products-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gs1.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\n- host: ref.gs1.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\n- host: world.openfoodfacts.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:07:01 2026 GMT\n  hsts: false\ndomains:\n- domain: gs1.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: openfoodfacts.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consumer-products/refs/heads/main/security/consumer-products-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Consumer Products
- CPG
- Product Data
- Retail
- GTIN
- Barcode
- Product Catalog
- PIM
- Syndication
- Schema.org Product
---
