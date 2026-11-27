---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hotspot.earth
  spf: true
hosts:
- cert_expires: Feb  8 03:44:10 2027 GMT
  host: hotspot.earth
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hotspot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hotspot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hotspot
provider_slug: hotspot-earth
slug: hotspot-earth-domain-security
source_filename: hotspot-earth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hotspot.earth\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 03:44:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hotspot.earth\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/hotspot-earth/security/hotspot-earth-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Creator Platform
- Monetization
- Maps
- Paywall
- Stripe
---
