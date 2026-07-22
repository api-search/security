---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: percent.com
  spf: true
hosts:
- cert_expires: Sep 16 21:16:05 2026 GMT
  host: percent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 19:48:34 2026 GMT
  host: portal.percent.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Percent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Percent, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Percent
provider_slug: percent
slug: percent-domain-security
source_filename: percent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: percent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 21:16:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal.percent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:48:34 2026 GMT\n  hsts: null\ndomains:\n- domain: percent.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/percent/refs/heads/main/security/percent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Private Credit
- Investing
- Debt Capital Markets
- Broker-Dealer
- Asset-Backed Securities
- Financial Services
---
