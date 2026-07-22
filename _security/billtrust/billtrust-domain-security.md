---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: billtrust.com
  spf: true
hosts:
- cert_expires: Aug 29 16:51:14 2026 GMT
  host: www.billtrust.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Billtrust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Billtrust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Billtrust
provider_slug: billtrust
slug: billtrust-domain-security
source_filename: billtrust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.billtrust.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:51:14 2026 GMT\n  hsts: false\ndomains:\n- domain: billtrust.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billtrust/refs/heads/main/security/billtrust-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Accounts Receivable
- B2B Payments
- Invoicing
- Cash Application
- Collections
- Order to Cash
---
