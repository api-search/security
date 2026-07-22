---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cashforce.com
  spf: true
hosts:
- cert_expires: Sep 14 06:29:53 2026 GMT
  host: cashforce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cashforce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cashforce, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cashforce
provider_slug: cashforce
slug: cashforce-domain-security
source_filename: cashforce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cashforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 06:29:53 2026 GMT\n  hsts: null\ndomains:\n- domain: cashforce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cashforce/refs/heads/main/security/cashforce-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Financial Services
- Cash Flow Forecasting
- Working Capital
- Treasury
- Cash Management
- Analytics
---
