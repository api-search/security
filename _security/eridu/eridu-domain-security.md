---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eridu.ai
  spf: true
hosts:
- cert_expires: Oct  9 16:51:43 2026 GMT
  host: eridu.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eridu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eridu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eridu
provider_slug: eridu
slug: eridu-domain-security
source_filename: eridu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eridu.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:51:43 2026 GMT\n  hsts: false\ndomains:\n- domain: eridu.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eridu/refs/heads/main/security/eridu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- AI Infrastructure
- Networking
- Semiconductors
- Data Center
- Silicon
- Network Switching
- Interconnect
- Hardware
- Content
---
