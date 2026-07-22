---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: avenue.app
  spf: false
hosts:
- cert_expires: Aug 21 16:18:44 2026 GMT
  host: avenue.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avenue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avenue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Avenue
provider_slug: avenue
slug: avenue-domain-security
source_filename: avenue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avenue.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:18:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: avenue.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avenue/refs/heads/main/security/avenue-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Cloud Saas
- Operations
- Observability
- Workflow Automation
- Alerting
- RevOps
- Task Queue
---
