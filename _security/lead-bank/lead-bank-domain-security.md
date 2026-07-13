---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lead.bank
  spf: true
hosts:
- cert_expires: Sep 23 00:58:37 2026 GMT
  host: lead.bank
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 12:24:08 2026 GMT
  host: docs.lead.bank
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: api.sandbox.lead.bank
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lead Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lead Bank, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lead Bank
provider_slug: lead-bank
slug: lead-bank-domain-security
source_filename: lead-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lead.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 00:58:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lead.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 12:24:08 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.sandbox.lead.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lead.bank\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lead-bank/refs/heads/main/security/lead-bank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Sponsor Bank
- Embedded Finance
- Banking as a Service
- Payments
- Lending
- Cards
- Deposits
---
