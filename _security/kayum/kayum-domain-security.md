---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kayum.mx
  spf: true
hosts:
- cert_expires: Aug 30 03:28:53 2026 GMT
  host: kayum.mx
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kayum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kayum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kayum
provider_slug: kayum
slug: kayum-domain-security
source_filename: kayum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kayum.mx\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 30 03:28:53 2026 GMT\n  hsts: null\ndomains:\n- domain: kayum.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kayum/refs/heads/main/security/kayum-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Insurance
- InsurTech
- Data Analytics
- Market Data
- Insurance Pricing
- Mexico
---
