---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: navatop.com
  spf: true
hosts:
- cert_expires: Feb  7 02:14:24 2027 GMT
  host: navatop.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NavaTOP Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NavaTOP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NavaTOP
provider_slug: navatop-com
slug: navatop-com-domain-security
source_filename: navatop-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: navatop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 02:14:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: navatop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/navatop-com/security/navatop-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Tools
- FreeSoftware
- Small Business
- Vietnam
- Open Source
---
