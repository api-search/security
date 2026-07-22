---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: themarketiq.com
  spf: false
hosts:
- cert_expires: Sep 20 15:40:00 2026 GMT
  host: themarketiq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Market Iq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Market IQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Market IQ
provider_slug: market-iq
slug: market-iq-domain-security
source_filename: market-iq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: themarketiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:40:00 2026 GMT\n  hsts: false\ndomains:\n- domain: themarketiq.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/market-iq/refs/heads/main/security/market-iq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Analytics
- Predictive Analytics
- Financial Services
- Banking
- Capital Markets
- Natural Language Processing
- Machine Learning
---
