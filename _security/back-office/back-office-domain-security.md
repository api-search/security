---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: finally.com
  spf: true
hosts:
- cert_expires: Sep 26 12:26:47 2026 GMT
  host: finally.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Back Office Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Back Office, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Back Office
provider_slug: back-office
slug: back-office-domain-security
source_filename: back-office-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finally.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 12:26:47 2026 GMT\n  hsts: false\ndomains:\n- domain: finally.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/back-office/refs/heads/main/security/back-office-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Accounting
- Bookkeeping
- Payroll
- Expense Management
- Accounts Payable
- Corporate Cards
- Invoicing
- Financial Automation
- AI Agents
---
