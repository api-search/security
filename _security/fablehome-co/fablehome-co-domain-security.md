---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fablehome.co
  spf: true
hosts:
- cert_expires: Jan 16 01:10:32 2027 GMT
  host: us.fablehome.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fablehome Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fable
provider_slug: fablehome-co
slug: fablehome-co-domain-security
source_filename: fablehome-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: us.fablehome.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 01:10:32 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: fablehome.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fablehome-co/security/fablehome-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- E-commerce
- Home Goods
- Design
- Sustainable
---
