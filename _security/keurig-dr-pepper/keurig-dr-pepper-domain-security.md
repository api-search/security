---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: keurigdrpepper.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: kdpproductfacts.com
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.keurigdrpepper.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 03:33:26 2026 GMT
  host: www.kdpproductfacts.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keurig Dr Pepper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keurig Dr Pepper, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Keurig Dr Pepper
provider_slug: keurig-dr-pepper
slug: keurig-dr-pepper-domain-security
source_filename: keurig-dr-pepper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.keurigdrpepper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\n- host: www.kdpproductfacts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 03:33:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: keurigdrpepper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: kdpproductfacts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keurig-dr-pepper/refs/heads/main/security/keurig-dr-pepper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Beverages
- Coffee
- Consumer Goods
- Fortune 500
- Single-Serve
---
