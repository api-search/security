---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: arrows.to
  spf: true
hosts:
- cert_expires: Jan 21 08:13:50 2027 GMT
  host: arrows.to
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arrows Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arrows, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Arrows
provider_slug: arrows
slug: arrows-domain-security
source_filename: arrows-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arrows.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 08:13:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arrows.to\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/arrows/security/arrows-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales
- AI
- Automation
- CRM
- SaaS
- Productivity
---
