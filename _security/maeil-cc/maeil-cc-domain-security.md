---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: maeil.cc
  spf: true
hosts:
- cert_expires: Dec 21 00:05:54 2026 GMT
  host: maeil.cc
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: maeil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for maeil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: maeil
provider_slug: maeil-cc
slug: maeil-cc-domain-security
source_filename: maeil-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maeil.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 00:05:54 2026 GMT\n  hsts: false\ndomains:\n- domain: maeil.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/maeil-cc/security/maeil-cc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Calendar
- SMS
- Scheduling
- AI Assistant
---
