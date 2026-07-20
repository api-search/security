---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: argalabs.com
  spf: true
hosts:
- cert_expires: Oct 14 22:17:57 2026 GMT
  host: docs.argalabs.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 17 06:17:17 2026 GMT
  host: api.argalabs.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Arga Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arga Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Arga Labs
provider_slug: arga-labs
slug: arga-labs-domain-security
source_filename: arga-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.argalabs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 14 22:17:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.argalabs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 17 06:17:17 2026 GMT\n  hsts: null\ndomains:\n- domain: argalabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arga-labs/refs/heads/main/security/arga-labs-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- API Testing
- Sandboxes
- Digital Twins
- AI Agents
- Developer Tools
- Testing Infrastructure
- CI/CD
- Browser Testing
- MCP
- Mock Services
---
