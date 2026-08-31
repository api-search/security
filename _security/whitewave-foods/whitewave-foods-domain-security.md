---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: danonewave.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: danone.com
  spf: true
hosts:
- cert_expires: Sep  5 12:03:09 2026 GMT
  host: www.danonewave.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.danone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whitewave Foods Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WhiteWave Foods, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: WhiteWave Foods
provider_slug: whitewave-foods
slug: whitewave-foods-domain-security
source_filename: whitewave-foods-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.danonewave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 12:03:09 2026 GMT\n  hsts: false\n- host: www.danone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: danonewave.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: danone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whitewave-foods/refs/heads/main/security/whitewave-foods-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food And Beverage
- Plant-Based
- Organic
- Consumer Goods
- Dairy
---
