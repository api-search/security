---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alitheon.com
  spf: true
hosts:
- cert_expires: Nov 24 19:03:53 2026 GMT
  host: alitheon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alitheon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alitheon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alitheon
provider_slug: alitheon
slug: alitheon-domain-security
source_filename: alitheon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alitheon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 19:03:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: alitheon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alitheon/refs/heads/main/security/alitheon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Anti‑Counterfeit
- Asset Management
- Supply Chain
- Physical Identity
- Optical AI
---
