---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jeremydevos.fr
  spf: true
hosts:
- cert_expires: Jan 27 19:42:25 2027 GMT
  host: jeremydevos.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jérémy Devos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jérémy Devos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jérémy Devos
provider_slug: jeremydevos-fr
slug: jeremydevos-fr-domain-security
source_filename: jeremydevos-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jeremydevos.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 19:42:25 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jeremydevos.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jeremydevos-fr/security/jeremydevos-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Magento
- Web Development
- France
- Software-as-a-Service
---
