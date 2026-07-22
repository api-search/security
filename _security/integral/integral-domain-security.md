---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: integral.com
  spf: true
hosts:
- cert_expires: Oct 17 13:18:00 2026 GMT
  host: www.integral.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Integral Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Integral, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Integral
provider_slug: integral
slug: integral-domain-security
source_filename: integral-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.integral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 13:18:00 2026 GMT\n  hsts: false\ndomains:\n- domain: integral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/integral/refs/heads/main/security/integral-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Foreign Exchange
- Trading
- Digital Assets
- Institutional
- Capital Markets
- Market Data
---
