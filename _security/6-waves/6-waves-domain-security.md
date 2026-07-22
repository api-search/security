---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 6waves.com
  spf: true
hosts:
- cert_expires: Oct 11 05:34:33 2026 GMT
  host: www.6waves.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 6 Waves Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 6 Waves, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 6 Waves
provider_slug: 6-waves
slug: 6-waves-domain-security
source_filename: 6-waves-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.6waves.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 05:34:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: 6waves.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6-waves/refs/heads/main/security/6-waves-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Games
- Mobile Games
- Game Publishing
- Gaming
- Entertainment
---
