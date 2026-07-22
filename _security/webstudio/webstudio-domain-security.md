---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: webstudio.is
  spf: true
hosts:
- cert_expires: Aug 26 06:37:35 2026 GMT
  host: webstudio.is
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Webstudio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webstudio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Webstudio
provider_slug: webstudio
slug: webstudio-domain-security
source_filename: webstudio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: webstudio.is\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:37:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: webstudio.is\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webstudio/refs/heads/main/security/webstudio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Website Builder
- No-Code
- Visual Development
- Web Design
- CMS
- Open Source
- CLI
- MCP
- Developer Tools
---
