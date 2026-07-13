---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: postali.app
  spf: false
hosts:
- cert_expires: Sep 16 04:49:22 2026 GMT
  host: postali.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Postali Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Postali, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Postali
provider_slug: postali
slug: postali-domain-security
source_filename: postali-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: postali.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:49:22 2026 GMT\n  hsts: false\ndomains:\n- domain: postali.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postali/refs/heads/main/security/postali-domain-security.yml
summary_line: TLSv1.3
tags:
- Geocoding
- Public APIs
---
