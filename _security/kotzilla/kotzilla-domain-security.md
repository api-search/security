---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kotzilla.io
  spf: true
hosts:
- cert_expires: Sep 26 23:54:56 2026 GMT
  host: kotzilla.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 19:06:21 2026 GMT
  host: doc.kotzilla.io
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 01:28:05 2026 GMT
  host: mcp.kotzilla.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kotzilla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kotzilla, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kotzilla
provider_slug: kotzilla
slug: kotzilla-domain-security
source_filename: kotzilla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kotzilla.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:54:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.kotzilla.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 19:06:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: mcp.kotzilla.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 01:28:05 2026 GMT\n  hsts: null\ndomains:\n- domain: kotzilla.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kotzilla/refs/heads/main/security/kotzilla-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Data
- Observability
- Monitoring
- Developer Tools
- Kotlin
- Android
- Mobile
- Dependency Injection
- Performance
- MCP
- Agents
---
