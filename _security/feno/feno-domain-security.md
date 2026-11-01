---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: feno.co
  spf: true
hosts:
- cert_expires: Jan  5 21:25:32 2027 GMT
  host: feno.co
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Feno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Feno, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Feno
provider_slug: feno
slug: feno-domain-security
source_filename: feno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: feno.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 21:25:32 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: feno.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/feno/security/feno-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Oral Care
- HealthTech
- Smartbrush
- AI
- Consumer Electronics
---
