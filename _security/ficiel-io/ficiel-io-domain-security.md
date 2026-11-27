---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ficiel.io
  spf: true
hosts:
- cert_expires: Dec 31 18:33:00 2026 GMT
  host: ficiel.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ficiel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ficiel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ficiel
provider_slug: ficiel-io
slug: ficiel-io-domain-security
source_filename: ficiel-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ficiel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 18:33:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ficiel.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ficiel-io/security/ficiel-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Messaging
- Sales
- Coaching
- Automation
---
