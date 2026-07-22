---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sav.money
  spf: true
hosts:
- cert_expires: Oct  3 15:12:32 2026 GMT
  host: sav.money
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sav Technologies Limited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sav Technologies Limited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sav Technologies Limited
provider_slug: sav-technologies-limited
slug: sav-technologies-limited-domain-security
source_filename: sav-technologies-limited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sav.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:12:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sav.money\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sav-technologies-limited/refs/heads/main/security/sav-technologies-limited-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Financial Services
- Savings
- Investing
- Wealth Management
- Gold
- Prepaid Card
- Personal Finance
- UAE
---
