---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: media2url.com
  spf: true
hosts:
- cert_expires: Nov 29 07:18:53 2026 GMT
  host: media2url.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Media2Url Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Media2URL Direct Media Delivery API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Media2URL Direct Media Delivery API
provider_slug: media2url
slug: media2url-domain-security
source_filename: media2url-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: media2url.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 07:18:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: media2url.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/media2url/refs/heads/main/security/media2url-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Media
- FileHosting
- DirectLinks
- Upload
---
