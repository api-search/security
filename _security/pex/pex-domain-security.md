---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: pex.com
  spf: true
hosts:
- cert_expires: Oct  4 07:54:51 2026 GMT
  host: pex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 16:18:47 2026 GMT
  host: docs.api.pex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 07:54:51 2026 GMT
  host: api.pex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pex, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Pex
provider_slug: pex
slug: pex-domain-security
source_filename: pex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:54:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.api.pex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 16:18:47 2026 GMT\n  hsts: false\n- host: api.pex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 07:54:51 2026 GMT\n  hsts: null\ndomains:\n- domain: pex.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pex/refs/heads/main/security/pex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Developer Tools
- Content Identification
- Digital Rights Management
- Music
- Audio Recognition
- Artificial Intelligence
- Content Recognition
- Media
- MCP
---
