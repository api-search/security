---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: capitolis.com
  spf: true
hosts:
- cert_expires: Sep 14 17:32:31 2026 GMT
  host: capitolis.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capitolis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capitolis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Capitolis
provider_slug: capitolis
slug: capitolis-domain-security
source_filename: capitolis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capitolis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 17:32:31 2026 GMT\n  hsts: false\ndomains:\n- domain: capitolis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capitolis/refs/heads/main/security/capitolis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Capital Markets
- FinTech
- Capital Optimization
- Portfolio Optimization
- Derivatives
- Institutional Investing
---
