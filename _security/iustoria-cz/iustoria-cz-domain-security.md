---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: iustoria.cz
  spf: true
hosts:
- cert_expires: Jan  1 03:53:48 2027 GMT
  host: iustoria.cz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: IUSTORIA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IUSTORIA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: IUSTORIA
provider_slug: iustoria-cz
slug: iustoria-cz-domain-security
source_filename: iustoria-cz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iustoria.cz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 03:53:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iustoria.cz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/iustoria-cz/security/iustoria-cz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Law
- Legal Services
- Czech Republic
- Brno
- Business Law
---
