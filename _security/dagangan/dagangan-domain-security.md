---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dagangan.com
  spf: true
hosts:
- cert_expires: Sep  1 02:15:31 2026 GMT
  host: dagangan.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dagangan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dagangan, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dagangan
provider_slug: dagangan
slug: dagangan-domain-security
source_filename: dagangan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dagangan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 02:15:31 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: dagangan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dagangan/refs/heads/main/security/dagangan-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- E-Commerce
- Wholesale
- Logistics
- Retail
- Supply Chain
- Rural Commerce
- Indonesia
---
