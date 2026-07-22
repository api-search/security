---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amie.so
  spf: true
hosts:
- cert_expires: Sep 20 16:51:30 2026 GMT
  host: www.amie.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amie
provider_slug: amie
slug: amie-domain-security
source_filename: amie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amie.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:51:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amie.so\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amie/refs/heads/main/security/amie-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Calendar
- Productivity
- Meetings
- AI Assistant
- Scheduling
- Tasks
- Notes
- MCP
---
