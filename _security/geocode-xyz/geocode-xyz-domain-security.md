---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: geocode.xyz
  spf: true
hosts:
- cert_expires: Oct  7 02:48:52 2026 GMT
  host: geocode.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geocode Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geocode.xyz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Geocode.xyz
provider_slug: geocode-xyz
slug: geocode-xyz-domain-security
source_filename: geocode-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geocode.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 02:48:52 2026 GMT\n  hsts: false\ndomains:\n- domain: geocode.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocode-xyz/refs/heads/main/security/geocode-xyz-domain-security.yml
summary_line: TLSv1.3
tags:
- Geocoding
- Public APIs
---
