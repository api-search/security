---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bit.cloud
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bit.dev
  spf: true
hosts:
- cert_expires: Oct 12 19:02:33 2026 GMT
  host: bit.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 22:17:53 2026 GMT
  host: bit.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 15:00:55 2026 GMT
  host: api.v2.bit.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bit
provider_slug: bit
slug: bit-domain-security
source_filename: bit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bit.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 19:02:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bit.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:17:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.v2.bit.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 15:00:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bit.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: bit.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bit/refs/heads/main/security/bit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Devops
- Component Development
- Frontend
- Monorepo
- npm
- GraphQL
- CLI
- MCP
- Developer Tools
- AI Agents
---
