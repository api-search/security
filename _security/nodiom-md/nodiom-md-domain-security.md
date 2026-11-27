---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nodiom.md
  spf: false
hosts:
- cert_expires: Jan  7 10:18:26 2027 GMT
  host: nodiom.md
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nodiom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nodiom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Nodiom
provider_slug: nodiom-md
slug: nodiom-md-domain-security
source_filename: nodiom-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nodiom.md\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 10:18:26 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nodiom.md\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nodiom-md/security/nodiom-md-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Collaboration
- Task Management
- Automation
- Company
---
