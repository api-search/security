---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: 18birdies.com
  spf: true
  spf_record: v=spf1 include:servers.mcsv.net include:_spf.google.com include:mailgun.org ?all
hosts:
- cert_expires: Dec 26 12:56:59 2026 GMT
  host: 18birdies.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: api.18birdies.com
  hsts: false
  hsts_max_age: null
  https: true
  note: Private mobile-app backend behind an AWS ELB. GET / returns HTTP 403 (Jetty); every documented discovery path returns 404. Not a published API surface.
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: 18Birdies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 18Birdies, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: 18Birdies
provider_slug: 18birdies
slug: 18birdies-domain-security
source_filename: 18birdies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + the app backend host api.18birdies.com\nnote: >-\n  Baseline written by 0-working/probe-domain-security.py, then extended by hand with two\n  probes the script did not cover: the SPF record (the script recorded spf: false, but\n  `dig +short 18birdies.com TXT` returns a v=spf1 record — corrected below), and the mobile\n  app backend host api.18birdies.com, which is not in apis.yml because 18Birdies publishes\n  no API and so has no apis[] entry.\nhosts:\n- host: 18birdies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 12:56:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.18birdies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: false\n  hsts_max_age: null\n  note: >-\n    Private mobile-app backend behind an AWS ELB. GET / returns HTTP 403 (Jetty); every\n    documented discovery path returns 404. Not\
  \ a published API surface.\ndomains:\n- domain: 18birdies.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:servers.mcsv.net include:_spf.google.com include:mailgun.org ?all\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/18birdies/refs/heads/main/security/18birdies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Golf
- Sports
- Mobile Applications
- Location
- Geolocation
- Mapping
- Consumer
- Fitness
- Social
- Analytics
- Tournaments
- Subscriptions
---
