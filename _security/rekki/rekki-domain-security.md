---
api_specs:
- filename: rekki-supplier-api-openapi-original.json
  format: json
  label: REKKI Supplier API
  slug: rekki-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rekki/refs/heads/main/openapi/rekki-supplier-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rekki.com
  spf: true
hosts:
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: rekki.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: api.rekki.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Rekki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REKKI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: REKKI
provider_slug: rekki
slug: rekki-domain-security
source_filename: rekki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rekki.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rekki.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: rekki.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rekki/refs/heads/main/security/rekki-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Food
- Wholesale
- Ordering
- Restaurants
- Supply Chain
- Catalog
- Orders
- eCommerce
---
