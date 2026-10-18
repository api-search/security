---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: c6bank.com.br
  spf: true
hosts:
- cert_expires: Jan 21 18:40:32 2027 GMT
  host: www.c6bank.com.br
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: C6 Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for C6 Bank, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: C6 Bank
provider_slug: c6-bank
slug: c6-bank-domain-security
source_filename: c6-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.c6bank.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:40:32 2027 GMT\n  hsts: null\ndomains:\n- domain: c6bank.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/c6-bank/refs/heads/main/security/c6-bank-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Banking
- Fintech
- Digital Bank
- Brazil
---
