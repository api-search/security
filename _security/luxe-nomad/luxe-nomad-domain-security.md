---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: theluxenomad.com
  spf: true
hosts:
- cert_expires: Sep 17 08:46:23 2026 GMT
  host: theluxenomad.com
  hsts: true
  hsts_max_age: 1800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Luxe Nomad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luxe Nomad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Luxe Nomad
provider_slug: luxe-nomad
slug: luxe-nomad-domain-security
source_filename: luxe-nomad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: theluxenomad.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 08:46:23 2026 GMT\n  hsts: true\n  hsts_max_age: 1800\ndomains:\n- domain: theluxenomad.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luxe-nomad/refs/heads/main/security/luxe-nomad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Travel
- Hospitality
- Villas
- Booking
- Luxury Travel
---
