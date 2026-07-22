---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: keurig.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: keurigdrpepper.com
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: www.keurig.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.keurigdrpepper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keurig Green Mountain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keurig Green Mountain, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Keurig Green Mountain
provider_slug: keurig-green-mountain
slug: keurig-green-mountain-domain-security
source_filename: keurig-green-mountain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.keurig.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: null\n- host: www.keurigdrpepper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: keurig.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: keurigdrpepper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keurig-green-mountain/refs/heads/main/security/keurig-green-mountain-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Beverages
- Coffee
- Consumer Goods
- Historical
- Single-Serve
---
