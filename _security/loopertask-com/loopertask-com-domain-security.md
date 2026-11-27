---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: loopertask.com
  spf: true
hosts:
- cert_expires: Feb  4 20:22:49 2027 GMT
  host: loopertask.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LooperTask Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LooperTask, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LooperTask
provider_slug: loopertask-com
slug: loopertask-com-domain-security
source_filename: loopertask-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loopertask.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 20:22:49 2027 GMT\n  hsts: false\ndomains:\n- domain: loopertask.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/loopertask-com/security/loopertask-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Time Tracking
- Invoicing
- AI Automation
- Studio
- Agencies
---
