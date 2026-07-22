---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kenvue.com
  spf: true
hosts:
- cert_expires: Sep  8 12:41:11 2026 GMT
  host: www.kenvue.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kenvue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kenvue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kenvue
provider_slug: kenvue
slug: kenvue-domain-security
source_filename: kenvue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kenvue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 12:41:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kenvue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kenvue/refs/heads/main/security/kenvue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consumer Health
- Personal Care
- Pharmaceuticals
- Skincare
- Fortune 500
---
