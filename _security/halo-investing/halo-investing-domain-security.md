---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dmarc_record: v=DMARC1; p=none; rua=mailto:ndmdixvq@rua.eu.dmarcmanager.app,mailto:dmarc@haloinvesting.com; adkim=r; aspf=r; pct=100
  dnssec: false
  domain: haloinvesting.com
  spf: true
hosts:
- cert_expires: Sep 25 05:16:55 2026 GMT
  host: haloinvesting.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  role: marketing site (WordPress)
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: notes.haloinvesting.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  role: authenticated advisor platform (Halo Notes) — AWS ALB, Next.js
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Halo Investing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Halo Investing, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Halo Investing
provider_slug: halo-investing
slug: halo-investing-domain-security
source_filename: halo-investing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts (probe-domain-security.py, plus a\n  manual curl pass that recovered the HSTS headers the scripted HEAD request missed)\nhosts:\n- host: haloinvesting.com\n  role: marketing site (WordPress)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 05:16:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  hsts_preload: false\n- host: notes.haloinvesting.com\n  role: authenticated advisor platform (Halo Notes) — AWS ALB, Next.js\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\ndomains:\n- domain: haloinvesting.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dmarc_record: 'v=DMARC1; p=none; rua=mailto:ndmdixvq@rua.eu.dmarcmanager.app,mailto:dmarc@haloinvesting.com;\n    adkim=r; aspf=r;\
  \ pct=100'\nnotes:\n- The apex domain publishes SPF and DMARC, but the DMARC policy is p=none (monitor\n  only, no enforcement), and there is no CAA record and no DNSSEC.\n- The authenticated platform host notes.haloinvesting.com carries the stronger posture\n  — HSTS with includeSubDomains and preload — while the marketing apex sets a bare\n  max-age with neither.\n- 'DNS caution for future rounds: *.haloinvesting.com is a wildcard A record pointing\n  at 52.73.145.146. Every unregistered subdomain (api., developer., apis., gateway.,\n  status., trust., security., mcp.) resolves and answers HTTP 502 with an HTML body.\n  Treat any such subdomain as a wildcard artifact, not a real host.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halo-investing/refs/heads/main/security/halo-investing-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial-Services
- Fintech
- WealthTech
- Investing
- Structured Notes
- Annuities
- Insurance
- Broker-Dealer
- Capital Markets
- Wealth Management
---
