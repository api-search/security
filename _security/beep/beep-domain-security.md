---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: justbeepit.com
  spf: true
hosts:
- cert_expires: Sep 29 04:15:25 2026 GMT
  host: justbeepit.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beep, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Beep
provider_slug: beep
slug: beep-domain-security
source_filename: beep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justbeepit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:15:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: justbeepit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beep/refs/heads/main/security/beep-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Collaboration
- Feedback
- Bug Reporting
- Website Review
- Productivity
- Browser Extension
- MCP
---
