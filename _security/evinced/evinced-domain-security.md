---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: evinced.com
  spf: true
hosts:
- cert_expires: Sep 30 10:18:36 2026 GMT
  host: www.evinced.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evinced Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for evinced, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: evinced
provider_slug: evinced
slug: evinced-domain-security
source_filename: evinced-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evinced.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:18:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: evinced.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evinced/refs/heads/main/security/evinced-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Accessibility
- Testing
- Quality Assurance
- Devops
- Web
- Mobile
- MCP
- SDK
- Artificial Intelligence
---
