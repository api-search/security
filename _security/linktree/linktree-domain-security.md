---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: linktr.ee
  spf: true
hosts:
- cert_expires: Nov 27 01:38:01 2026 GMT
  host: linktr.ee
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 24 13:43:28 2026 GMT
  host: mcp.linktr.ee
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 21 13:48:20 2026 GMT
  host: arbor.linktr.ee
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Linktree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linktree, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Linktree
provider_slug: linktree
slug: linktree-domain-security
source_filename: linktree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linktr.ee\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 27 01:38:01 2026 GMT\n  hsts: false\n- host: mcp.linktr.ee\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 24 13:43:28 2026 GMT\n  hsts: null\n- host: arbor.linktr.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 13:48:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: linktr.ee\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linktree/refs/heads/main/security/linktree-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Media
- Link in Bio
- Creator Economy
- Social Media
- Marketing
- Analytics
- MCP
- Agents
- Developer Tools
- Australia
---
