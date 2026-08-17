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
- cert_expires: Sep 28 02:33:15 2026 GMT
  host: linktr.ee
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 25 14:38:17 2026 GMT
  host: mcp.linktr.ee
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 22 12:35:18 2026 GMT
  host: arbor.linktr.ee
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linktree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linktree, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Linktree
provider_slug: linktree
slug: linktree-domain-security
source_filename: linktree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linktr.ee\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 02:33:15 2026 GMT\n  hsts: false\n- host: mcp.linktr.ee\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 25 14:38:17 2026 GMT\n  hsts: null\n- host: arbor.linktr.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 12:35:18 2026 GMT\n  hsts: false\ndomains:\n- domain: linktr.ee\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linktree/refs/heads/main/security/linktree-domain-security.yml
summary_line: TLSv1.2 · DMARC
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
- Design System
- Developer Tools
---
