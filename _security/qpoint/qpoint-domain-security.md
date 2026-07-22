---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qpoint.io
  spf: true
hosts:
- cert_expires: Oct  7 11:03:51 2026 GMT
  host: www.qpoint.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qpoint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qpoint, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Qpoint
provider_slug: qpoint
slug: qpoint-domain-security
source_filename: qpoint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qpoint.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 11:03:51 2026 GMT\n  hsts: false\ndomains:\n- domain: qpoint.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qpoint/refs/heads/main/security/qpoint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Security
- Observability
- eBPF
- Network Traffic
- Egress Control
- Agentic AI
- MCP
- gRPC
---
