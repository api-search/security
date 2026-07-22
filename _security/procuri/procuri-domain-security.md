---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: procuri.ai
  spf: false
hosts:
- cert_expires: Aug 31 08:14:57 2026 GMT
  host: www.procuri.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Procuri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Procuri, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Procuri
provider_slug: procuri
slug: procuri-domain-security
source_filename: procuri-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.procuri.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 08:14:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: procuri.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/procuri/refs/heads/main/security/procuri-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Procurement
- Sourcing
- Supply Chain
- Spend Management
- Contract Management
- AI Agents
- Automation
- Enterprise Software
---
