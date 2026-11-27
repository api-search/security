---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: grand.tennis
  spf: false
hosts:
- cert_expires: Feb  5 20:25:59 2027 GMT
  host: grand.tennis
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 4GRAND Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 4GRAND, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: 4GRAND
provider_slug: grand-tennis
slug: grand-tennis-domain-security
source_filename: grand-tennis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grand.tennis\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 20:25:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: grand.tennis\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/grand-tennis/security/grand-tennis-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Tennis
- Grand Slam
---
