---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: highbeam.co
  spf: true
hosts:
- cert_expires: Sep 23 03:17:03 2026 GMT
  host: highbeam.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Highbeam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Highbeam, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Highbeam
provider_slug: highbeam
slug: highbeam-domain-security
source_filename: highbeam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: highbeam.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 03:17:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: highbeam.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highbeam/refs/heads/main/security/highbeam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Banking
- Fintech
- Business Banking
- Financial Services
- E-commerce
- Working Capital
- Consumer Brands
---
