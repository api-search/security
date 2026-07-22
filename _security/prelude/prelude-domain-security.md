---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: originhq.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: www.originhq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 17:01:01 2026 GMT
  host: support.originhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: mcp.prod.originhq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prelude Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prelude, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Prelude
provider_slug: prelude
slug: prelude-domain-security
source_filename: prelude-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.originhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: support.originhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 17:01:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mcp.prod.originhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: originhq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prelude/refs/heads/main/security/prelude-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- AI Security
- AI Observability
- Endpoint Security
- AI Agents
- Model Context Protocol
- MCP
- Insight Partners
---
