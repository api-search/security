---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: osly.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pocketflow.ai
  spf: true
hosts:
- cert_expires: Nov  1 11:03:47 2026 GMT
  host: osly.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 04:29:22 2026 GMT
  host: api.pocketflow.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Osly, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Osly
provider_slug: osly
slug: osly-domain-security
source_filename: osly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: osly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 11:03:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.pocketflow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 04:29:22 2026 GMT\n  hsts: null\ndomains:\n- domain: osly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pocketflow.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osly/refs/heads/main/security/osly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Workflow Automation
- No-Code
- Agents
- Lead Generation
- Productivity
- Integration
- Low-Code
---
