---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dima.click
  spf: true
hosts:
- cert_expires: Jan 19 22:55:30 2027 GMT
  host: dima.click
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: dima.click Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dima.click, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: dima.click
provider_slug: dima-click
slug: dima-click-domain-security
source_filename: dima-click-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dima.click\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 22:55:30 2027 GMT\n  hsts: false\ndomains:\n- domain: dima.click\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dima-click/security/dima-click-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI Agents
- Voice Agents
- Automation
- Websites
- Conversational AI
- Agency
---
