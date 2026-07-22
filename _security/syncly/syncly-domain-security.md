---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: syncly.app
  spf: true
hosts:
- cert_expires: Sep 23 15:03:31 2026 GMT
  host: syncly.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Syncly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syncly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Syncly
provider_slug: syncly
slug: syncly-domain-security
source_filename: syncly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: syncly.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 15:03:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: syncly.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syncly/refs/heads/main/security/syncly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Social Intelligence
- Social Listening
- Customer Feedback
- Voice of Customer
- Creator Marketing
- Analytics
- Artificial Intelligence
- MCP
---
