---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: conviva.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: conviva.com
  spf: true
hosts:
- cert_expires: Oct 22 23:56:46 2026 GMT
  host: www.conviva.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 04:28:59 2026 GMT
  host: docs.conviva.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 14:12:32 2026 GMT
  host: api.conviva.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conviva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conviva, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Conviva
provider_slug: conviva
slug: conviva-domain-security
source_filename: conviva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.conviva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:56:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.conviva.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 04:28:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.conviva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 14:12:32 2026 GMT\n  hsts: null\ndomains:\n- domain: conviva.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: conviva.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conviva/refs/heads/main/security/conviva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Streaming
- Video
- Observability
- Monitoring
- Media
- Quality of Experience
- Real-Time
- Telemetry
- Agents
- MCP
- Company
---
