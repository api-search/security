---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sycamore.so
  spf: true
hosts:
- cert_expires: Aug 26 12:24:00 2026 GMT
  host: sycamore.so
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sycamore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sycamore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sycamore
provider_slug: sycamore
slug: sycamore-domain-security
source_filename: sycamore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sycamore.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 12:24:00 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: sycamore.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sycamore/refs/heads/main/security/sycamore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Agents
- Agent Operating System
- Enterprise Software
- Agent Governance
- Autonomous Agents
- Enterprise AI
---
