---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: primerevenue.com
  spf: true
hosts:
- cert_expires: Oct  6 08:31:02 2026 GMT
  host: primerevenue.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Primerevenue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PrimeRevenue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PrimeRevenue
provider_slug: primerevenue
slug: primerevenue-domain-security
source_filename: primerevenue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: primerevenue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:31:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: primerevenue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/primerevenue/refs/heads/main/security/primerevenue-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Supply Chain Finance
- Working Capital
- B2B Payments
- Receivables Finance
- Dynamic Discounting
- Fintech
- Financial Services
---
