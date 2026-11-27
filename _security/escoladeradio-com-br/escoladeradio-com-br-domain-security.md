---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: escoladeradio.com.br
  spf: true
hosts:
- cert_expires: Feb  2 05:54:04 2027 GMT
  host: escoladeradio.com.br
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Escola de Rádio TV & Web Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Escola de Rádio TV & Web, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Escola de Rádio TV & Web
provider_slug: escoladeradio-com-br
slug: escoladeradio-com-br-domain-security
source_filename: escoladeradio-com-br-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: escoladeradio.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 05:54:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: escoladeradio.com.br\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/escoladeradio-com-br/security/escoladeradio-com-br-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Media
- Broadcasting
- Training
- Brazil
- Company
---
