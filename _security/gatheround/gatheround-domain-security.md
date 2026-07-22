---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gatheround.com
  spf: true
hosts:
- cert_expires: Sep  5 10:13:46 2026 GMT
  host: gatheround.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gatheround Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gatheround, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Gatheround
provider_slug: gatheround
slug: gatheround-domain-security
source_filename: gatheround-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gatheround.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 10:13:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: gatheround.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gatheround/refs/heads/main/security/gatheround-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Video Conferencing
- Online Meetings
- Team Engagement
- Community
- Collaboration
- Employee Engagement
- Remote Work
---
