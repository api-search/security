---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amer-daniel.com
  spf: false
hosts:
- cert_expires: Jan 14 21:50:29 2027 GMT
  host: amer-daniel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amer Daniel Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daniel Amer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Daniel Amer
provider_slug: amer-daniel-com
slug: amer-daniel-com-domain-security
source_filename: amer-daniel-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amer-daniel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 21:50:29 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amer-daniel.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/amer-daniel-com/security/amer-daniel-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ingeniero Informático
- Consultoría
- Infraestructura
- Seguridad
- Criptoactivos
---
