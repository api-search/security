---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: repl.it
  spf: true
hosts:
- cert_expires: Jan  6 19:59:22 2027 GMT
  host: repl.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Repl It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Repl.it, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Repl.it
provider_slug: repl-it
slug: repl-it-domain-security
source_filename: repl-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: repl.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 19:59:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: repl.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/repl-it/security/repl-it-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- IDE
- Cloud
- Collaboration
- Education
- Enterprise
---
