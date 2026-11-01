---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: decibel.bio
  spf: true
hosts:
- cert_expires: Jan  5 16:04:51 2027 GMT
  host: www.decibel.bio
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Decibel Bio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Decibel Bio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Decibel Bio
provider_slug: decibel-bio
slug: decibel-bio-domain-security
source_filename: decibel-bio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.decibel.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 16:04:51 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: decibel.bio\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/decibel-bio/security/decibel-bio-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Agriculture
- AgTech
- Biotechnology
- Real-Time Data
---
