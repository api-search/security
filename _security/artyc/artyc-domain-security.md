---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: shipartyc.com
  spf: true
hosts:
- cert_expires: Jan 20 18:54:55 2027 GMT
  host: shipartyc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Artyc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artyc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Artyc
provider_slug: artyc
slug: artyc-domain-security
source_filename: artyc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shipartyc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 18:54:55 2027 GMT\n  hsts: null\ndomains:\n- domain: shipartyc.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/artyc/security/artyc-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Technology
- Digital-Asset-Management
- Workflow-Automation
- APIs
- Integration
- Analytics
---
