---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aruna.id
  spf: true
hosts:
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: aruna.id
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aruna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aruna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aruna
provider_slug: aruna
slug: aruna-domain-security
source_filename: aruna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aruna.id\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aruna.id\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aruna/refs/heads/main/security/aruna-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Marketplace
- Fisheries
- Seafood
- Supply Chain
- E-Commerce
- Indonesia
- Sustainability
---
