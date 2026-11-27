---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloziq.com
  spf: true
hosts:
- cert_expires: Jan 14 00:26:41 2027 GMT
  host: cloziq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloziq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloziq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloziq
provider_slug: cloziq-com
slug: cloziq-com-domain-security
source_filename: cloziq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloziq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 00:26:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cloziq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cloziq-com/security/cloziq-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Sales Agent
- Instagram
- Facebook Messenger
- Direct Messaging
- Appointment-Setting
- Sales Automation
- MCP
---
