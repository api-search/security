---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mspstuff.io
  spf: false
hosts:
- cert_expires: Nov 28 03:43:55 2026 GMT
  host: mspstuff.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mspstuff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutomatedMSP,, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: AutomatedMSP,
provider_slug: mspstuff
slug: mspstuff-domain-security
source_filename: mspstuff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mspstuff.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 03:43:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mspstuff.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mspstuff/security/mspstuff-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- MSP
- Artificial Intelligence
- Automation
- Software-as-a-Service
---
