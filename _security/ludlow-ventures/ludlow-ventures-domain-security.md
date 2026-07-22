---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ludlowventures.com
  spf: false
hosts:
- cert_expires: Oct 14 19:20:38 2026 GMT
  host: www.ludlowventures.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ludlow Ventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ludlow Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Ludlow Ventures
provider_slug: ludlow-ventures
slug: ludlow-ventures-domain-security
source_filename: ludlow-ventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ludlowventures.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 19:20:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ludlowventures.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ludlow-ventures/refs/heads/main/security/ludlow-ventures-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Venture Capital
- Early Stage
- Seed
- Startups
- Investment
- Detroit
---
