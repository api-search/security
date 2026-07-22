---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: superlist.com
  spf: true
hosts:
- cert_expires: Sep 26 09:07:24 2026 GMT
  host: superlist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:59:59 2026 GMT
  host: www.superlist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 05:58:21 2026 GMT
  host: app.superlist.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superlist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superlist, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Superlist
provider_slug: superlist
slug: superlist-domain-security
source_filename: superlist-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superlist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 09:07:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.superlist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.superlist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 05:58:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: superlist.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superlist/refs/heads/main/security/superlist-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Project Management Sector
- Task Management
- Productivity
- To-Do Lists
- Collaboration
- MCP
- Agents
- AI Assistant
---
