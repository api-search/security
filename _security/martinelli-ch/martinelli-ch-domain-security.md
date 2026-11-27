---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: martinelli.ch
  spf: true
hosts:
- cert_expires: Jan 19 12:48:54 2027 GMT
  host: martinelli.ch
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Martinelli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Martinelli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Martinelli
provider_slug: martinelli-ch
slug: martinelli-ch-domain-security
source_filename: martinelli-ch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: martinelli.ch\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 12:48:54 2027 GMT\n  hsts: false\ndomains:\n- domain: martinelli.ch\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/martinelli-ch/security/martinelli-ch-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Consulting
- Software Development
- Java
- Artificial Intelligence
- Modernization
---
