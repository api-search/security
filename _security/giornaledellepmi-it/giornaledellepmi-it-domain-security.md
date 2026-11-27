---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: giornaledellepmi.it
  spf: true
hosts:
- cert_expires: Jan 20 18:15:43 2027 GMT
  host: giornaledellepmi.it
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Il Giornale delle PMI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Il Giornale delle PMI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Il Giornale delle PMI
provider_slug: giornaledellepmi-it
slug: giornaledellepmi-it-domain-security
source_filename: giornaledellepmi-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: giornaledellepmi.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 18:15:43 2027 GMT\n  hsts: false\ndomains:\n- domain: giornaledellepmi.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/giornaledellepmi-it/security/giornaledellepmi-it-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Magazine
- Media
- Italian
- Small Business
- Business
---
