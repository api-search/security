---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coralswarm.com
  spf: true
hosts:
- cert_expires: Dec 29 03:35:16 2026 GMT
  host: coralswarm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CoralSwarm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CoralSwarm, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CoralSwarm
provider_slug: coralswarm-com
slug: coralswarm-com-domain-security
source_filename: coralswarm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coralswarm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 03:35:16 2026 GMT\n  hsts: false\ndomains:\n- domain: coralswarm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/coralswarm-com/security/coralswarm-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Organizational Memory
- Knowledge Management
- AI Agents
- MCP
- Search
- Productivity
- Collaboration
---
