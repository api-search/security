---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: balance.re
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: balance.re
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Balance Re Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Balance Re, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Balance Re
provider_slug: balance-re
slug: balance-re-domain-security
source_filename: balance-re-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: balance.re\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: balance.re\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/balance-re/refs/heads/main/security/balance-re-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Reinsurance
- Insurance
- Insurtech
- Life Insurance
- Asset-Liability Management
- Pension
- Fintech
- Germany
---
