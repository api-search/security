---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: osly.ai
  spf: true
hosts:
- cert_expires: Sep  1 21:51:51 2026 GMT
  host: osly.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Osly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Osly
provider_slug: osly
slug: osly-domain-security
source_filename: osly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: osly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 21:51:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: osly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
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
---
