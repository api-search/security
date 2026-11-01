---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cybera.io
  spf: true
hosts:
- cert_expires: Jan  1 22:17:05 2027 GMT
  host: www.cybera.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cybera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cybera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cybera
provider_slug: cybera
slug: cybera-domain-security
source_filename: cybera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cybera.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 22:17:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cybera.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cybera/security/cybera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Technology
- Platform
- Data
---
