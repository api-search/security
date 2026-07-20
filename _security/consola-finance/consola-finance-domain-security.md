---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: request.finance
  spf: true
hosts:
- cert_expires: Sep 10 02:25:47 2026 GMT
  host: docs.request.finance
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 08:02:16 2026 GMT
  host: api.request.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Consola Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Consola Finance, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Consola Finance
provider_slug: consola-finance
slug: consola-finance-domain-security
source_filename: consola-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.request.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 02:25:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.request.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 08:02:16 2026 GMT\n  hsts: null\ndomains:\n- domain: request.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consola-finance/refs/heads/main/security/consola-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Accounting
- Digital Assets
- Web3 Finance
- Accounts Payable
- Accounts Receivable
- Invoicing
- Payroll
- Bookkeeping
- Blockchain
---
