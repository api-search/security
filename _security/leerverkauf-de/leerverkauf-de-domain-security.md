---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: leerverkauf.de
  spf: true
hosts:
- cert_expires: Jan  9 21:19:58 2027 GMT
  host: leerverkauf.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: leerverkauf-de Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for leerverkauf-de, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: leerverkauf-de
provider_slug: leerverkauf-de
slug: leerverkauf-de-domain-security
source_filename: leerverkauf-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leerverkauf.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 21:19:58 2027 GMT\n  hsts: false\ndomains:\n- domain: leerverkauf.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/leerverkauf-de/security/leerverkauf-de-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
