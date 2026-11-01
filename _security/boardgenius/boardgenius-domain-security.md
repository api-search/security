---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boardgenius.io
  spf: true
hosts:
- cert_expires: Dec 29 23:06:53 2026 GMT
  host: boardgenius.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boardgenius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Board Genius, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Board Genius
provider_slug: boardgenius
slug: boardgenius-domain-security
source_filename: boardgenius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boardgenius.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:06:53 2026 GMT\n  hsts: false\ndomains:\n- domain: boardgenius.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/boardgenius/security/boardgenius-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- SaaS
- Integration
- Automation
- Project-Management
---
