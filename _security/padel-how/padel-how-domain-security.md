---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: padel.how
  spf: true
hosts:
- cert_expires: Jan  1 04:14:31 2027 GMT
  host: padel.how
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: padel.how Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for padel.how, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: padel.how
provider_slug: padel-how
slug: padel-how-domain-security
source_filename: padel-how-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: padel.how\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 04:14:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: padel.how\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/padel-how/security/padel-how-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Reviews
- Padel
- Racket Finder
- Rankings
---
