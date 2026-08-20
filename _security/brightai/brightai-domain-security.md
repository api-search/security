---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bright.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: stateful.world
  spf: true
hosts:
- cert_expires: Oct 20 23:27:46 2026 GMT
  host: www.bright.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: public.stateful.world
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brightai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BrightAI, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BrightAI
provider_slug: brightai
slug: brightai-domain-security
source_filename: brightai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bright.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:27:46 2026 GMT\n  hsts: false\n- host: public.stateful.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: bright.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: stateful.world\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightai/refs/heads/main/security/brightai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Physical AI
- Industrial IoT
- Infrastructure Monitoring
- Predictive Maintenance
- Edge AI
- Foundation Models
- MCP
- Energy and Utilities
- Water and Wastewater
---
