---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: naftiko.io
  spf: true
hosts:
- cert_expires: Oct 28 18:42:20 2026 GMT
  host: naftiko.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Naftiko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Naftiko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Naftiko
provider_slug: naftiko
slug: naftiko-domain-security
source_filename: naftiko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: naftiko.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 18:42:20 2026 GMT\n  hsts: false\ndomains:\n- domain: naftiko.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/naftiko/refs/heads/main/security/naftiko-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Data
- API Integration
- API Governance
- MCP
- Agent Skills
- Open-Source
- Developer Tools
- API Specification
- Spec-Driven Integration
- Capability Engine
- API Linting
---
