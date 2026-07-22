---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boardable.com
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: boardable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boardable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boardable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Boardable
provider_slug: boardable
slug: boardable-domain-security
source_filename: boardable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boardable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boardable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boardable/refs/heads/main/security/boardable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Board Management
- Governance
- Nonprofit
- Meetings
- Board Portal
- Collaboration
- No Public API
---
