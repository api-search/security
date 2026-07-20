---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fenbeitong.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: www.fenbeitong.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fenbeitong Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fenbeitong, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fenbeitong
provider_slug: fenbeitong
slug: fenbeitong-domain-security
source_filename: fenbeitong-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fenbeitong.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: fenbeitong.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fenbeitong/refs/heads/main/security/fenbeitong-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- Spend Management
- Expense Management
- Corporate Travel
- Payments
- Procurement
- China
---
