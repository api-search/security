---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moderne.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: moderne.io
  spf: true
hosts:
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: moderne.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 04:39:48 2026 GMT
  host: docs.moderne.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: api.app.moderne.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moderne Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moderne, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moderne
provider_slug: moderne
slug: moderne-domain-security
source_filename: moderne-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moderne.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: false\n- host: docs.moderne.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:39:48 2026 GMT\n  hsts: false\n- host: api.app.moderne.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: moderne.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: moderne.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moderne/refs/heads/main/security/moderne-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Developer Tools
- Code Transformation
- Automated Refactoring
- Code Migration
- Security Patching
- OpenRewrite
- Static Analysis
- Code Governance
- DevOps
- GraphQL
- AI Agents
- MCP
---
