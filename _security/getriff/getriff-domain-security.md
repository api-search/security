---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getriff.co
  spf: true
hosts:
- cert_expires: Sep 17 22:36:23 2026 GMT
  host: getriff.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getriff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for getriff, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: getriff
provider_slug: getriff
slug: getriff-domain-security
source_filename: getriff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getriff.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:36:23 2026 GMT\n  hsts: false\ndomains:\n- domain: getriff.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getriff/refs/heads/main/security/getriff-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Video Conferencing
- Team Collaboration
- Remote Work
- Voice
- Productivity
- Desktop Software
---
