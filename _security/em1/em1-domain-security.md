---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: em1.com
  spf: true
hosts:
- cert_expires: Nov 30 20:35:04 2026 GMT
  host: em1.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Em1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EM1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: EM1
provider_slug: em1
slug: em1-domain-security
source_filename: em1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: em1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 20:35:04 2026 GMT\n  hsts: false\ndomains:\n- domain: em1.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/em1/security/em1-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Emergency Management
- AI Tools
- Safety
- Compliance
---
