---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alloyx.com
  spf: false
hosts:
- cert_expires: Oct 22 05:27:30 2026 GMT
  host: www.alloyx.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alloyx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AlloyX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AlloyX
provider_slug: alloyx
slug: alloyx-domain-security
source_filename: alloyx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alloyx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 05:27:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: alloyx.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloyx/refs/heads/main/security/alloyx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Stablecoin
- Digital Tokens
- Compliance
- Blockchain
- Regulated Finance
---
