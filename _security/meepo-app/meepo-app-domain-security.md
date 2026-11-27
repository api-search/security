---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: meepo.app
  spf: true
hosts:
- cert_expires: Jan 15 01:00:31 2027 GMT
  host: meepo.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meepo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meepo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Meepo
provider_slug: meepo-app
slug: meepo-app-domain-security
source_filename: meepo-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meepo.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 01:00:31 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: meepo.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/meepo-app/security/meepo-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Content
- Marketing
- Artificial Intelligence
- Design
- Automation
- Company
---
