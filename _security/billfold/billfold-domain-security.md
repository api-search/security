---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: billfold.tech
  spf: true
hosts:
- cert_expires: Dec 12 03:58:57 2026 GMT
  host: www.billfold.tech
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Billfold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Billfold, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Billfold
provider_slug: billfold
slug: billfold-domain-security
source_filename: billfold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.billfold.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 03:58:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: billfold.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billfold/refs/heads/main/security/billfold-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Event
- Point-of-Sale
- RFID
- Cashless
---
