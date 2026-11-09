---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blitzbuchen.de
  spf: true
hosts:
- cert_expires: Jan  8 19:31:17 2027 GMT
  host: blitzbuchen.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blitzbuchen De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlitzBuchen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BlitzBuchen
provider_slug: blitzbuchen-de
slug: blitzbuchen-de-domain-security
source_filename: blitzbuchen-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blitzbuchen.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 19:31:17 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: blitzbuchen.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blitzbuchen-de/security/blitzbuchen-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Germany
- LastMinute
- Packages
- Car Rental
---
