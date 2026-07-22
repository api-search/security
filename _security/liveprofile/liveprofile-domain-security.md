---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: liveprofile.com
  spf: false
hosts:
- cert_expires: Sep 14 15:15:23 2026 GMT
  host: liveprofile.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liveprofile Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liveprofile, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Liveprofile
provider_slug: liveprofile
slug: liveprofile-domain-security
source_filename: liveprofile-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liveprofile.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:15:23 2026 GMT\n  hsts: false\ndomains:\n- domain: liveprofile.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liveprofile/refs/heads/main/security/liveprofile-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Messaging
- Chat
- Communication
- Mobile
- Consumer
---
