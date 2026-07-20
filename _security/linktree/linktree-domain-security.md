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
- cert_expires: Aug 26 15:33:15 2026 GMT
  host: mcp.linktr.ee
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Linktree Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linktree, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Linktree
provider_slug: linktree
slug: linktree-domain-security
source_filename: linktree-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linktr.ee\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 02:33:15 2026 GMT\n  hsts: false\n- host: mcp.linktr.ee\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 26 15:33:15 2026 GMT\n  hsts: null\ndomains:\n- domain: linktr.ee\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
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
---
