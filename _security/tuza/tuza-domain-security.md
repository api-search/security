---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tuza.ai
  spf: true
hosts:
- cert_expires: Sep 11 05:04:42 2026 GMT
  host: www.tuza.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tuza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tuza, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tuza
provider_slug: tuza
slug: tuza-domain-security
source_filename: tuza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tuza.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:04:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tuza.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tuza/refs/heads/main/security/tuza-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Banking
- AI Agents
- Agentic AI
- Automation
- Workflow Automation
- United Kingdom
---
