---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reevo.ai
  spf: true
hosts:
- cert_expires: Aug 31 10:48:02 2026 GMT
  host: www.reevo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reevo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reevo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reevo
provider_slug: reevo
slug: reevo-domain-security
source_filename: reevo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reevo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 10:48:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: reevo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reevo/refs/heads/main/security/reevo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Sales
- CRM
- Revenue Operations
- Sales Automation
- Lead Generation
---
