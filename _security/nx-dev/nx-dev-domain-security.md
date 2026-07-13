---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nx.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nrwl.io
  spf: true
hosts:
- cert_expires: Sep 21 11:24:33 2026 GMT
  host: nx.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 05:49:40 2026 GMT
  host: nrwl.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nx Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nx, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Nx
provider_slug: nx-dev
slug: nx-dev-domain-security
source_filename: nx-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nx.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 11:24:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: nrwl.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:49:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nx.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nrwl.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nx-dev/refs/heads/main/security/nx-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Monorepo
- Build
- BuildSystem
- TaskRunner
- DependencyGraph
- Cache
- RemoteCache
- CI
- DistributedExecution
- DeveloperTools
- DeveloperExperience
- IDE
- AI
- Agents
- MCP
- ModelContextProtocol
- TypeScript
- JavaScript
- Rust
- OpenSource
---
