---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cequence.ai
  spf: true
hosts:
- cert_expires: Sep 26 17:38:02 2026 GMT
  host: www.cequence.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:42:56 2026 GMT
  host: helpdesk.cequence.ai
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cequence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cequence Security, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cequence Security
provider_slug: cequence
slug: cequence-domain-security
source_filename: cequence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cequence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:38:02 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: helpdesk.cequence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:42:56 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\ndomains:\n- domain: cequence.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cequence/refs/heads/main/security/cequence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Protection
- API Discovery
- API Security
- Application Security
- Attack Surface
- Bot Management
- Business Logic Abuse
- CNAPP
- Cybersecurity
- Fraud
- Unified API Protection
---
