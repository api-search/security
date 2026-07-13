---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: westernsouthern.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gerberlife.com
  spf: true
hosts:
- cert_expires: Sep  6 15:09:22 2026 GMT
  host: www.westernsouthern.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 15:09:22 2026 GMT
  host: www.gerberlife.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 14:57:51 2026 GMT
  host: www.touchstoneinvestments.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Western And Southern Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for western-and-southern-financial, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: western-and-southern-financial
provider_slug: western-and-southern-financial
slug: western-and-southern-financial-domain-security
source_filename: western-and-southern-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.westernsouthern.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:09:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.gerberlife.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:09:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.touchstoneinvestments.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 14:57:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: westernsouthern.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gerberlife.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-and-southern-financial/refs/heads/main/security/western-and-southern-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
