---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: asaak.com
  spf: true
hosts:
- cert_expires: Aug 10 04:59:51 2026 GMT
  host: asaak.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asaak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asaak, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Asaak
provider_slug: asaak
slug: asaak-domain-security
source_filename: asaak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asaak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 04:59:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: asaak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asaak/refs/heads/main/security/asaak-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Fintech
- Lending
- Asset Financing
- Financial Services
- Working Capital
- Africa
- Uganda
- Mobility
---
