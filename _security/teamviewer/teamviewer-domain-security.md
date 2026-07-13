---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: teamviewer.com
  spf: true
hosts:
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.teamviewer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 23:59:59 2026 GMT
  host: webapi.teamviewer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teamviewer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TeamViewer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TeamViewer
provider_slug: teamviewer
slug: teamviewer-domain-security
source_filename: teamviewer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.teamviewer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: webapi.teamviewer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: teamviewer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamviewer/refs/heads/main/security/teamviewer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Remote Access
- Remote Support
- Remote Desktop
- IT Management
- Endpoint Management
- Unified Endpoint Management
---
