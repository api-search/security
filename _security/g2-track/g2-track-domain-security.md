---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bettercloud.com
  spf: true
hosts:
- cert_expires: Oct  7 10:20:02 2026 GMT
  host: www.bettercloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: G2 Track Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for G2 Track, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: G2 Track
provider_slug: g2-track
slug: g2-track-domain-security
source_filename: g2-track-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bettercloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:20:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bettercloud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/g2-track/refs/heads/main/security/g2-track-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Contract Management
- SaaS Management
- Spend Optimization
---
