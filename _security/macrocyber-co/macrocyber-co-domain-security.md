---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: macrocyber.co
  spf: false
hosts:
- cert_expires: Jan  2 22:49:13 2027 GMT
  host: macrocyber.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MacroCyber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MacroCyber, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: MacroCyber
provider_slug: macrocyber-co
slug: macrocyber-co-domain-security
source_filename: macrocyber-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: macrocyber.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 22:49:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: macrocyber.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/macrocyber-co/security/macrocyber-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Security
- Attack Surface
- Mapping
- Monitoring
---
