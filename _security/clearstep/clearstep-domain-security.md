---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: clearstep.health
  spf: true
hosts:
- cert_expires: Sep 14 02:49:29 2026 GMT
  host: clearstep.health
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clearstep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clearstep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Clearstep
provider_slug: clearstep
slug: clearstep-domain-security
source_filename: clearstep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clearstep.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 02:49:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clearstep.health\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearstep/refs/heads/main/security/clearstep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Digital Health
- Clinical Triage
- Symptom Checker
- Patient Navigation
- Care Navigation
- AI Agents
- Scheduling
- Health Systems
---
