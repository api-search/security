---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leadpages.com
  spf: true
hosts:
- cert_expires: Sep 14 03:31:31 2026 GMT
  host: leadpages.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.leadpages.com
  https: false
- cert_expires: Sep 14 03:31:31 2026 GMT
  host: mcp.leadpages.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Leadpages Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leadpages, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Leadpages
provider_slug: leadpages
slug: leadpages-domain-security
source_filename: leadpages-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leadpages.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:31:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.leadpages.com\n  https: false\n- host: mcp.leadpages.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 03:31:31 2026 GMT\n  hsts: null\ndomains:\n- domain: leadpages.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leadpages/refs/heads/main/security/leadpages-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Landing Pages
- Marketing
- Conversion Optimization
- A/B Testing
- Website Builder
- Lead Generation
- Content Management
- Agents
- Analytics
---
