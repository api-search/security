---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: autoleap.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: myautoleap.com
  spf: true
hosts:
- cert_expires: Oct  6 03:34:31 2026 GMT
  host: autoleap.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 04:17:57 2026 GMT
  host: developers.myautoleap.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: partnerapi.myautoleap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autoleap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoLeap, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AutoLeap
provider_slug: autoleap
slug: autoleap-domain-security
source_filename: autoleap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autoleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:34:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.myautoleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:17:57 2026 GMT\n  hsts: false\n- host: partnerapi.myautoleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: autoleap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: myautoleap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoleap/refs/heads/main/security/autoleap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Auto Repair
- Shop Management
- Automotive
- Partner API
- Vertical SaaS
---
