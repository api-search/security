---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infinera.com
  spf: false
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.infinera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Infinera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infinera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Infinera
provider_slug: infinera
slug: infinera-domain-security
source_filename: infinera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infinera.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: infinera.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infinera/refs/heads/main/security/infinera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hardware
- Optical Networking
- Telecommunications
- Networking
- DWDM
- Transport Network
- Network Automation
---
