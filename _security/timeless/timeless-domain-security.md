---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: timeless.investments
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.timeless.investments
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Timeless Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Timeless, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Timeless
provider_slug: timeless
slug: timeless-domain-security
source_filename: timeless-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.timeless.investments\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: timeless.investments\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/timeless/refs/heads/main/security/timeless-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Fintech
- Collectibles
- Alternative Assets
- Fractional Ownership
- Investing
- Mobile App
---
