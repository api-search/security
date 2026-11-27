---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: askqa.app
  spf: true
hosts:
- cert_expires: Jan 20 09:13:16 2027 GMT
  host: askqa.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ASKQA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ASKQA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ASKQA
provider_slug: askqa-app
slug: askqa-app-domain-security
source_filename: askqa-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: askqa.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 09:13:16 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: askqa.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/askqa-app/security/askqa-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- WhatsApp bots
- Workflows
- Reporting
- Customer Service
- Integration
- Business Software
---
