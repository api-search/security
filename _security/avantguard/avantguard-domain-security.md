---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: avantguardinc.com
  spf: false
hosts:
- cert_expires: Nov 22 04:44:25 2026 GMT
  host: www.avantguardinc.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avantguard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AvantGuard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AvantGuard
provider_slug: avantguard
slug: avantguard-domain-security
source_filename: avantguard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avantguardinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 04:44:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: avantguardinc.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avantguard/refs/heads/main/security/avantguard-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Antimicrobial
- Biotechnology
- Healthcare
- Startups
---
