---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: meniga.com
  spf: true
hosts:
- cert_expires: Oct  6 13:56:19 2026 GMT
  host: www.meniga.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meniga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meniga, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Meniga
provider_slug: meniga
slug: meniga-domain-security
source_filename: meniga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meniga.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 13:56:19 2026 GMT\n  hsts: false\ndomains:\n- domain: meniga.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meniga/refs/heads/main/security/meniga-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Digital Banking
- Personal Finance Management
- Open Banking
- Transaction Enrichment
- Financial Services
- Banking
- SDK
---
