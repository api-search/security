---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unremind.me
  spf: true
hosts:
- cert_expires: Jan 11 12:17:14 2027 GMT
  host: unremind.me
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Unremind Me Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for unremind-me, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: unremind-me
provider_slug: unremind-me
slug: unremind-me-domain-security
source_filename: unremind-me-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unremind.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 12:17:14 2027 GMT\n  hsts: false\ndomains:\n- domain: unremind.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/unremind-me/security/unremind-me-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Productivity
- Reminders
- Context-Aware
- AI
---
