---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: animaapp.com
  spf: true
hosts:
- cert_expires: Mar 29 23:59:59 2027 GMT
  host: animaapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anima Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anima, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Anima
provider_slug: animaapp-com
slug: animaapp-com-domain-security
source_filename: animaapp-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: animaapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: animaapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/animaapp-com/security/animaapp-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Design
- Code Generation
- Platform
---
