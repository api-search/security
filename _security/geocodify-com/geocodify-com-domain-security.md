---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geocodify.com
  spf: true
hosts:
- cert_expires: Aug 23 18:16:15 2026 GMT
  host: geocodify.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geocodify Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geocodify.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Geocodify.com
provider_slug: geocodify-com
slug: geocodify-com-domain-security
source_filename: geocodify-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geocodify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:16:15 2026 GMT\n  hsts: false\ndomains:\n- domain: geocodify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocodify-com/refs/heads/main/security/geocodify-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geocoding
- Public APIs
---
