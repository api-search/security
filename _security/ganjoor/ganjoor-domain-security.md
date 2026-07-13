---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ganjoor.net
  spf: true
hosts:
- cert_expires: Sep  8 04:31:36 2026 GMT
  host: api.ganjoor.net
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ganjoor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ganjoor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ganjoor
provider_slug: ganjoor
slug: ganjoor-domain-security
source_filename: ganjoor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.ganjoor.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  8 04:31:36 2026 GMT\n  hsts: false\ndomains:\n- domain: ganjoor.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ganjoor/refs/heads/main/security/ganjoor-domain-security.yml
summary_line: TLSv1.2
tags:
- Books
- Public APIs
---
