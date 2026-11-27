---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cloche.dev
  spf: true
hosts:
- cert_expires: Jan 12 17:31:57 2027 GMT
  host: cloche.dev
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloche Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloche, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cloche
provider_slug: cloche-dev
slug: cloche-dev-domain-security
source_filename: cloche-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloche.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 17:31:57 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cloche.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cloche-dev/security/cloche-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- MCP
- Ai Apps
- Governance
- Low-Code
- Internal Tools
- Agents
---
