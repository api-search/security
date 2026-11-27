---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: markboard.work
  spf: true
hosts:
- cert_expires: Jan  1 20:26:46 2027 GMT
  host: markboard.work
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Markboard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Markboard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Markboard
provider_slug: markboard-work
slug: markboard-work-domain-security
source_filename: markboard-work-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: markboard.work\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 20:26:46 2027 GMT\n  hsts: false\ndomains:\n- domain: markboard.work\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/markboard-work/security/markboard-work-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Kanban
- Markdown
- Artificial Intelligence
- Self-Hosted
---
