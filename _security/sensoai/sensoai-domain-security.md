---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: senso.ai
  spf: true
hosts:
- cert_expires: Sep 14 12:50:23 2026 GMT
  host: senso.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: docs.senso.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 31 08:41:21 2026 GMT
  host: apiv2.senso.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sensoai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Senso.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Senso.ai
provider_slug: sensoai
slug: sensoai-domain-security
source_filename: sensoai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: senso.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:50:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.senso.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: false\n- host: apiv2.senso.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 08:41:21 2026 GMT\n  hsts: null\ndomains:\n- domain: senso.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sensoai/refs/heads/main/security/sensoai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Knowledge Base
- AI Agents
- Content Generation
- Semantic Search
- Generative Engine Optimization
- Verified Context
- Agentic Web
- MCP
---
