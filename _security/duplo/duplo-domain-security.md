---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tryduplo.com
  spf: true
hosts:
- cert_expires: Sep 11 01:32:22 2026 GMT
  host: tryduplo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: docs.tryduplo.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: atlas.tryduplo.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Duplo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Duplo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Duplo
provider_slug: duplo
slug: duplo-domain-security
source_filename: duplo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryduplo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 01:32:22 2026 GMT\n  hsts: false\n- host: docs.tryduplo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\n- host: atlas.tryduplo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: tryduplo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/duplo/refs/heads/main/security/duplo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- FinTech
- Payments
- B2B Payments
- Cross-Border Payments
- Expense Management
- Virtual Accounts
- E-Invoicing
- Foreign Exchange
- Africa
- Nigeria
---
