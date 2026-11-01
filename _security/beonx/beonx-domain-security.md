---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beonx.com
  spf: true
hosts:
- cert_expires: Dec 29 08:42:27 2026 GMT
  host: beonx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beonx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BeonX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BeonX
provider_slug: beonx
slug: beonx-domain-security
source_filename: beonx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beonx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 08:42:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: beonx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/beonx/security/beonx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Revenue-Management
- Hospitality
- SaaS
---
