---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usenotch.ai
  spf: true
hosts:
- cert_expires: Nov  1 02:32:44 2026 GMT
  host: www.usenotch.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: app.usenotch.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sesame Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sesame Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sesame Labs
provider_slug: sesame-labs
slug: sesame-labs-domain-security
source_filename: sesame-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usenotch.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 02:32:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.usenotch.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: usenotch.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sesame-labs/refs/heads/main/security/sesame-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Advertising
- Video
- Marketing
- Generative AI
- MCP
- Agents
---
