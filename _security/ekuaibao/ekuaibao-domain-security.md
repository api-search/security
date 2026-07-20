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
- cert_expires: Feb  7 09:15:01 2027 GMT
  host: docs.ekuaibao.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  7 09:15:01 2027 GMT
  host: app.ekuaibao.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ekuaibao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ekuaibao, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ekuaibao
provider_slug: ekuaibao
slug: ekuaibao-domain-security
source_filename: ekuaibao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ekuaibao.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  7 09:15:01 2027 GMT\n  hsts: false\n- host: docs.ekuaibao.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 09:15:01 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: app.ekuaibao.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 09:15:01 2027 GMT\n  hsts: null\ndomains:\n- domain: ekuaibao.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ekuaibao/refs/heads/main/security/ekuaibao-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Enterprise
- Expense Management
- Spend Management
- Travel and Expense
- Reimbursement
- Finance
- Accounting
- Invoicing
- SaaS
- China
---
