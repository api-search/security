---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: greaterthan.eu
  spf: true
hosts:
- cert_expires: Nov 20 09:22:49 2026 GMT
  host: greaterthan.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Greater Than Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Greater Than, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Greater Than
provider_slug: greater-than
slug: greater-than-domain-security
source_filename: greater-than-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: greaterthan.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 09:22:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: greaterthan.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greater-than/refs/heads/main/security/greater-than-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Risk Intelligence
- Road Safety
- Climate Impact
- AI
---
