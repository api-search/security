---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: folhamatic.com.br
  spf: true
hosts:
- host: www.folhamatic.com.br
  https: false
kind: domain-security
layout: security
method: probed
name: Folhamatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Folhamatic, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Folhamatic
provider_slug: folhamatic
slug: folhamatic-domain-security
source_filename: folhamatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.folhamatic.com.br\n  https: false\ndomains:\n- domain: folhamatic.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/folhamatic/refs/heads/main/security/folhamatic-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Accounting
- Payroll
- Tax
- Fiscal
- ERP
- Business Management
- Brazil
- Software
- Sage
---
