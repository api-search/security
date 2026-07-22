---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: quantive.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: workboard.com
  spf: true
hosts:
- cert_expires: Sep 25 17:37:14 2026 GMT
  host: quantive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 06:18:38 2026 GMT
  host: www.workboard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 19:50:02 2026 GMT
  host: www.myworkboard.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quantive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quantive, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Quantive
provider_slug: quantive
slug: quantive-domain-security
source_filename: quantive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quantive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:37:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.workboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 06:18:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.myworkboard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 19:50:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: quantive.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: workboard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quantive/refs/heads/main/security/quantive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Business Applications
- OKR
- Strategy Execution
- Goal Management
- Performance Management
- SaaS
---
