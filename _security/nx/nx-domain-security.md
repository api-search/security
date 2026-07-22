---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nx.dev
  spf: true
hosts:
- cert_expires: Sep 21 11:24:33 2026 GMT
  host: nx.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nx
provider_slug: nx
slug: nx-domain-security
source_filename: nx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nx.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 11:24:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nx.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nx/refs/heads/main/security/nx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Build System
- Monorepo
- Developer Tools
- CI/CD
- Continuous Integration
- Caching
- Command Line Interface
- Model Context Protocol
- JavaScript
- TypeScript
- DevOps
---
