---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: horizon3.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: horizon3ai.com
  spf: true
hosts:
- cert_expires: Sep  5 05:04:21 2026 GMT
  host: horizon3.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 22:02:38 2026 GMT
  host: docs.horizon3.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: api.gateway.horizon3ai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Horizon3Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Horizon3.ai, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Horizon3.ai
provider_slug: horizon3ai
slug: horizon3ai-domain-security
source_filename: horizon3ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: horizon3.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 05:04:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.horizon3.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 22:02:38 2026 GMT\n  hsts: false\n- host: api.gateway.horizon3ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: horizon3.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: horizon3ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/horizon3ai/refs/heads/main/security/horizon3ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Penetration Testing
- Autonomous Pentesting
- Attack Surface Management
- Exposure Management
- Vulnerability Management
- GraphQL
- Offensive Security
---
