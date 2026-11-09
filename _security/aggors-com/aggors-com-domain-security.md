---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aggors.com
  spf: true
hosts:
- cert_expires: Jan  4 23:52:35 2027 GMT
  host: aggors.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aggors Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aggors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aggors
provider_slug: aggors-com
slug: aggors-com-domain-security
source_filename: aggors-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aggors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:52:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aggors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aggors-com/security/aggors-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- MerchantEvidence
- Transparency
- Tools
---
