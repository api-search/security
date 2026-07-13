---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: picsum.photos
  spf: false
hosts:
- cert_expires: Sep 25 09:37:52 2026 GMT
  host: picsum.photos
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lorem Picsum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lorem Picsum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Lorem Picsum
provider_slug: lorem-picsum
slug: lorem-picsum-domain-security
source_filename: lorem-picsum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: picsum.photos\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 09:37:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: picsum.photos\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lorem-picsum/refs/heads/main/security/lorem-picsum-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Photography
- Public APIs
---
