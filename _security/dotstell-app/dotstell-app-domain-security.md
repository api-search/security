---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dotstell.app
  spf: true
hosts:
- cert_expires: Jan  5 23:35:32 2027 GMT
  host: dotstell.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dotstell App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dotstell-app, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: dotstell-app
provider_slug: dotstell-app
slug: dotstell-app-domain-security
source_filename: dotstell-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dotstell.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:35:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dotstell.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/dotstell-app/security/dotstell-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Knowledge Graph
- Personal Knowledge Management
- Productivity
- Note Taking
- AI Integration
---
