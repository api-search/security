---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spenny.com
  spf: false
hosts:
- cert_expires: Sep 26 06:27:17 2026 GMT
  host: spenny.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spenny Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spenny, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Spenny
provider_slug: spenny
slug: spenny-domain-security
source_filename: spenny-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spenny.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:27:17 2026 GMT\n  hsts: false\ndomains:\n- domain: spenny.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spenny/refs/heads/main/security/spenny-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Personal Finance
- Micro-Investing
- Savings
- Mutual Funds
- Digital Gold
- India
- Consumer App
---
