---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: webinarjam.com
  spf: true
hosts:
- cert_expires: Aug 12 14:00:39 2026 GMT
  host: www.webinarjam.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 11:32:47 2026 GMT
  host: documentation.webinarjam.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 18:06:57 2026 GMT
  host: api.webinarjam.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Webinarjam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WebinarJam, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: WebinarJam
provider_slug: webinarjam
slug: webinarjam-domain-security
source_filename: webinarjam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.webinarjam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 14:00:39 2026 GMT\n  hsts: false\n- host: documentation.webinarjam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 11:32:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.webinarjam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 18:06:57 2026 GMT\n  hsts: null\ndomains:\n- domain: webinarjam.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webinarjam/refs/heads/main/security/webinarjam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Webinars
- Marketing
- Live Events
- Automated Webinars
- Lead Generation
- SaaS
---
