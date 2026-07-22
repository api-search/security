---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: i2x.ai
  spf: true
hosts:
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: www.i2x.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: I2X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for i2x, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: i2x
provider_slug: i2x
slug: i2x-domain-security
source_filename: i2x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.i2x.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: i2x.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/i2x/refs/heads/main/security/i2x-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Enterprise Software
- Conversation Intelligence
- Contact Center
- Speech Recognition
- Real-Time AI
- Sales Enablement
- Compliance
- Germany
---
