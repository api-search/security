---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: putitforward.com
  spf: true
hosts:
- cert_expires: Dec 27 06:56:15 2026 GMT
  host: putitforward.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Putitforward Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Put it Forward, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Put it Forward
provider_slug: putitforward
slug: putitforward-domain-security
source_filename: putitforward-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: putitforward.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 06:56:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: putitforward.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/putitforward/security/putitforward-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automation
- AI
- Enterprise
- Integration
---
