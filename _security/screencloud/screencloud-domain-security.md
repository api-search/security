---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: screencloud.com
  spf: true
hosts:
- cert_expires: Sep 21 05:19:43 2026 GMT
  host: screencloud.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: developer.screencloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: studio.screencloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Screencloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ScreenCloud, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ScreenCloud
provider_slug: screencloud
slug: screencloud-domain-security
source_filename: screencloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: screencloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:19:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.screencloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\n- host: studio.screencloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: screencloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/screencloud/refs/heads/main/security/screencloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Signage
- Screens
- Content Management
- GraphQL
- Media
- Playlists
- Displays
---
