---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: plantanapp.com
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: plantanapp.com
  hsts: true
  hsts_max_age: 778000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Plant An App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plant an App, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Plant an App
provider_slug: plant-an-app
slug: plant-an-app-domain-security
source_filename: plant-an-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plantanapp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 778000\ndomains:\n- domain: plantanapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plant-an-app/refs/heads/main/security/plant-an-app-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Low-Code
- No-Code
- Application Development
- Workflow Automation
- Case Management
- Government
- Platform
---
