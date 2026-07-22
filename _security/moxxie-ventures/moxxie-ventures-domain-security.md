---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: moxxie.vc
  spf: true
hosts:
- cert_expires: Sep 29 10:29:27 2026 GMT
  host: www.moxxie.vc
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moxxie Ventures Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moxxie Ventures, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Moxxie Ventures
provider_slug: moxxie-ventures
slug: moxxie-ventures-domain-security
source_filename: moxxie-ventures-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moxxie.vc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:29:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: moxxie.vc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moxxie-ventures/refs/heads/main/security/moxxie-ventures-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Venture Capital
- Investment
- Seed Stage
- Early Stage
- Fund
- Vertical AI
---
