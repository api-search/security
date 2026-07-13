---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apiip.net
  spf: true
hosts:
- cert_expires: Aug 12 22:47:35 2026 GMT
  host: apiip.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apiip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apiip, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Apiip
provider_slug: apiip
slug: apiip-domain-security
source_filename: apiip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiip.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 22:47:35 2026 GMT\n  hsts: false\ndomains:\n- domain: apiip.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiip/refs/heads/main/security/apiip-domain-security.yml
summary_line: TLSv1.3
tags:
- Geocoding
- Public APIs
---
