---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ploy.ai
  spf: true
hosts:
- cert_expires: Sep 24 04:48:00 2026 GMT
  host: ploy.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ploy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ploy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ploy
provider_slug: ploy
slug: ploy-domain-security
source_filename: ploy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ploy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 04:48:00 2026 GMT\n  hsts: false\ndomains:\n- domain: ploy.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ploy/refs/heads/main/security/ploy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing
- Marketing Automation
- Artificial Intelligence
- AI Agents
- SEO
- Website Builder
- Growth
- Advertising
---
