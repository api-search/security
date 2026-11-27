---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hooksend.app
  spf: true
hosts:
- cert_expires: Dec 28 19:44:36 2026 GMT
  host: hooksend.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HookSend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HookSend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HookSend
provider_slug: hooksend-app
slug: hooksend-app-domain-security
source_filename: hooksend-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hooksend.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 19:44:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hooksend.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hooksend-app/security/hooksend-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Instagram
- Automation
- Artificial Intelligence
- Social Commerce
- Software-as-a-Service
---
