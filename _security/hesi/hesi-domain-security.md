---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ekuaibao.com
  spf: true
hosts:
- cert_expires: Feb  7 09:15:01 2027 GMT
  host: www.ekuaibao.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hesi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hesi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hesi
provider_slug: hesi
slug: hesi-domain-security
source_filename: hesi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ekuaibao.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  7 09:15:01 2027 GMT\n  hsts: false\ndomains:\n- domain: ekuaibao.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hesi/refs/heads/main/security/hesi-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Enterprise
- Expense Management
- Spend Management
- Finance
- SaaS
- Fintech
- Business Travel
- Reimbursement
- China
---
