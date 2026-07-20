---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: groupthink.com
  spf: true
hosts:
- cert_expires: Sep 28 23:02:00 2026 GMT
  host: groupthink.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.groupthink.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Groupthink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groupthink, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Groupthink
provider_slug: groupthink
slug: groupthink-domain-security
source_filename: groupthink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: groupthink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 23:02:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.groupthink.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: groupthink.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groupthink/refs/heads/main/security/groupthink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SaaS
- Meetings
- Transcription
- Note Taking
- Relationship Intelligence
- MCP
- AI Assistant
- Productivity
- CRM
---
