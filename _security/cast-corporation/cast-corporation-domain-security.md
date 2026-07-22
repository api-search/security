---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: cast.app
  spf: true
hosts:
- cert_expires: Sep 16 22:33:51 2026 GMT
  host: cast.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cast Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cast Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Cast Corporation
provider_slug: cast-corporation
slug: cast-corporation-domain-security
source_filename: cast-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cast.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 22:33:51 2026 GMT\n  hsts: false\ndomains:\n- domain: cast.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cast-corporation/refs/heads/main/security/cast-corporation-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Customer Success
- Artificial Intelligence
- AI Agents
- Revenue Operations
- SaaS
- Automation
- Post-Sales
---
