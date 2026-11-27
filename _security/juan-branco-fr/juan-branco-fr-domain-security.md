---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: juan-branco.fr
  spf: true
hosts:
- cert_expires: Jan  8 00:36:18 2027 GMT
  host: juan-branco.fr
  hsts: true
  hsts_max_age: 16000000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Juan Branco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juan Branco, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Juan Branco
provider_slug: juan-branco-fr
slug: juan-branco-fr-domain-security
source_filename: juan-branco-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: juan-branco.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 00:36:18 2027 GMT\n  hsts: true\n  hsts_max_age: 16000000\ndomains:\n- domain: juan-branco.fr\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/juan-branco-fr/security/juan-branco-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Law
- Biography
- Publications
- France
- Legal
---
