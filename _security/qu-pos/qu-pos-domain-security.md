---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qubeyond.com
  spf: true
hosts:
- cert_expires: Jan  8 23:31:30 2027 GMT
  host: www.qubeyond.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qu Pos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qu POS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qu POS
provider_slug: qu-pos
slug: qu-pos-domain-security
source_filename: qu-pos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qubeyond.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:31:30 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: qubeyond.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qu-pos/refs/heads/main/security/qu-pos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- POS
- Restaurant Technology
- Unified Commerce
- Kitchen Management
- Payments
- Channel Management
- Data Reporting
---
