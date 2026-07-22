---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: akto.io
  spf: true
hosts:
- cert_expires: Aug 23 23:59:59 2026 GMT
  host: www.akto.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akto, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Akto
provider_slug: akto
slug: akto-domain-security
source_filename: akto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akto.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: akto.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akto/refs/heads/main/security/akto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API Security
- Security
- API Security Testing
- DAST
- API Discovery
- AI Security
- MCP Security
- Open Source
- DevSecOps
- Governance
---
