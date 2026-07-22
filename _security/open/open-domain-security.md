---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: open.money
  spf: true
hosts:
- cert_expires: Dec  8 05:18:17 2026 GMT
  host: open.money
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Open
provider_slug: open
slug: open-domain-security
source_filename: open-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: open.money\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 05:18:17 2026 GMT\n  hsts: null\ndomains:\n- domain: open.money\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open/refs/heads/main/security/open-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Banking
- Business Banking
- Neobank
- SME
- Payments
- Accounting
- Payroll
- India
---
