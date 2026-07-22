---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: motilaloswal.com
  spf: true
hosts:
- cert_expires: Jan  4 07:26:25 2027 GMT
  host: www.motilaloswal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Motilal Oswal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motilal Oswal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Motilal Oswal
provider_slug: motilal-oswal
slug: motilal-oswal-domain-security
source_filename: motilal-oswal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.motilaloswal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 07:26:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: motilaloswal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motilal-oswal/refs/heads/main/security/motilal-oswal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Financial Services
- Brokerage
- Wealth Management
- Investing
- Stock Market
- Mutual Funds
- India
---
