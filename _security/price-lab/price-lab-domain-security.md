---
api_specs:
- filename: price-lab-openapi.yml
  format: yaml
  label: Price Lab API
  slug: price-lab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/price-lab/refs/heads/main/openapi/price-lab-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pricelabsolutions.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Aug 22 12:18:30 2026 GMT
  host: pricelabsolutions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: price-lab.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 12:54:17 2026 GMT
  host: backend.pricelab.com.pe
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Price Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Price Lab, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Price Lab
provider_slug: price-lab
slug: price-lab-domain-security
source_filename: price-lab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pricelabsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 12:18:30 2026 GMT\n  hsts: false\n- host: price-lab.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: backend.pricelab.com.pe\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 12:54:17 2026 GMT\n  hsts: null\ndomains:\n- domain: pricelabsolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/price-lab/refs/heads/main/security/price-lab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Pricing
- Retail
- E-commerce
- Competitive Intelligence
- Price Optimization
- Artificial Intelligence
- Electronic Shelf Labels
- Latin America
---
