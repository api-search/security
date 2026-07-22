---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jubileemedia.com
  spf: true
hosts:
- cert_expires: Sep 14 20:12:14 2026 GMT
  host: jubileemedia.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jubilee Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jubilee Inc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jubilee Inc
provider_slug: jubilee-inc
slug: jubilee-inc-domain-security
source_filename: jubilee-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jubileemedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:12:14 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: jubileemedia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jubilee-inc/refs/heads/main/security/jubilee-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- Video
- Entertainment
- Content Production
- Social Media
- YouTube
---
