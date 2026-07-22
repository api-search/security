---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: basebuild.com
  spf: true
hosts:
- cert_expires: Sep 25 18:16:19 2026 GMT
  host: basebuild.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Basebuild Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basebuild, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Basebuild
provider_slug: basebuild
slug: basebuild-domain-security
source_filename: basebuild-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: basebuild.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 18:16:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: basebuild.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basebuild/refs/heads/main/security/basebuild-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Construction
- Real Estate
- Artificial Intelligence
- Project Management
- Productivity
- Meetings
- Knowledge Base
---
