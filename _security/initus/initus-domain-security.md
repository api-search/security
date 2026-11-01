---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: initus.io
  spf: true
hosts:
- cert_expires: Nov  8 11:16:30 2026 GMT
  host: initus.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Initus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Initus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Initus
provider_slug: initus
slug: initus-domain-security
source_filename: initus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: initus.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 11:16:30 2026 GMT\n  hsts: false\ndomains:\n- domain: initus.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/initus/security/initus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Integration
- Workflow Automation
- AI
- Consulting
- ERP
- CRM
- E‑commerce
---
