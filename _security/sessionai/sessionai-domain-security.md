---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sessionai.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zineone.com
  spf: true
hosts:
- cert_expires: Oct 15 19:32:40 2026 GMT
  host: sessionai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 15:45:22 2026 GMT
  host: devguide.zineone.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: cloud.zineone.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sessionai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Session AI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Session AI
provider_slug: sessionai
slug: sessionai-domain-security
source_filename: sessionai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sessionai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:32:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: devguide.zineone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 15:45:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloud.zineone.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: sessionai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: zineone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sessionai/refs/heads/main/security/sessionai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Ecommerce
- Retail
- Personalization
- Marketing
- Agentic AI
- Decisioning
- Customer Data
- Events
- Real Time
- MCP
---
