---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: avataar.ai
  spf: true
hosts:
- cert_expires: Nov 30 09:12:24 2026 GMT
  host: www.avataar.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avataar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avataar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Avataar
provider_slug: avataar
slug: avataar-domain-security
source_filename: avataar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avataar.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 09:12:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: avataar.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avataar/refs/heads/main/security/avataar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Enterprise
- Automation
- AgenticAI
- Bengaluru
---
