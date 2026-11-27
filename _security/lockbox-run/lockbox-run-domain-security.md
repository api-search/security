---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lockbox.run
  spf: false
hosts:
- cert_expires: Jan  3 21:24:48 2027 GMT
  host: lockbox.run
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lockbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lockbox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Lockbox
provider_slug: lockbox-run
slug: lockbox-run-domain-security
source_filename: lockbox-run-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lockbox.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 21:24:48 2027 GMT\n  hsts: null\ndomains:\n- domain: lockbox.run\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lockbox-run/security/lockbox-run-domain-security.yml
summary_line: TLSv1.3
tags:
- Security
- Encryption
- Secrets
- CLI
- Artificial Intelligence
---
