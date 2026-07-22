---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rexnord.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: regalrexnord.com
  spf: true
hosts:
- cert_expires: Sep 15 19:17:25 2026 GMT
  host: www.rexnord.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 22:25:57 2026 GMT
  host: www.regalrexnord.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rexnord Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rexnord, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rexnord
provider_slug: rexnord
slug: rexnord-domain-security
source_filename: rexnord-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rexnord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:17:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.regalrexnord.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:25:57 2026 GMT\n  hsts: false\ndomains:\n- domain: rexnord.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: regalrexnord.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rexnord/refs/heads/main/security/rexnord-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Industrial Manufacturing
- Motion Control
- Water Management
- Bearings
- Couplings
- Fortune 1000
---
