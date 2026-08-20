---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: keepface.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: keepface.ai
  spf: false
hosts:
- cert_expires: Aug 21 18:23:27 2026 GMT
  host: keepface.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 19:13:09 2026 GMT
  host: help.keepface.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 09:18:12 2026 GMT
  host: api.keepface.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keepface Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KeepFace, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: KeepFace
provider_slug: keepface
slug: keepface-domain-security
source_filename: keepface-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keepface.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:23:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.keepface.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 19:13:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.keepface.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 09:18:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: keepface.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: keepface.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keepface/refs/heads/main/security/keepface-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Influencer Marketing
- Creator Economy
- Marketing
- Social-Media
- Affiliate Marketing
- Advocacy
- Campaign Management
- MCP
- AI Agents
- Attribution
- Webhook
---
