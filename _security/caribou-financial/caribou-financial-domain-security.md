---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cariboufinancial.com
  spf: true
hosts:
- cert_expires: Feb 19 21:31:30 2027 GMT
  host: www.cariboufinancial.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caribou Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caribou Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Caribou Financial
provider_slug: caribou-financial
slug: caribou-financial-domain-security
source_filename: caribou-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cariboufinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 21:31:30 2027 GMT\n  hsts: false\ndomains:\n- domain: cariboufinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caribou-financial/refs/heads/main/security/caribou-financial-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fintech
- AutoLoans
- Refinancing
- ConsumerFinance
---
