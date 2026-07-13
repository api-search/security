---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: geokeo.com
  spf: false
hosts:
- cert_expires: Sep 19 02:24:29 2026 GMT
  host: geokeo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geokeo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geokeo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Geokeo
provider_slug: geokeo
slug: geokeo-domain-security
source_filename: geokeo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geokeo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 02:24:29 2026 GMT\n  hsts: false\ndomains:\n- domain: geokeo.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geokeo/refs/heads/main/security/geokeo-domain-security.yml
summary_line: TLSv1.3
tags:
- Geocoding
- Public APIs
---
