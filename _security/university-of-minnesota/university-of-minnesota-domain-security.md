---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: umn.edu
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
hosts:
- cert_expires: Aug 24 05:47:55 2026 GMT
  host: twin-cities.umn.edu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: sites.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: integration-boomi.umn.edu
  https: false
kind: domain-security
layout: security
method: probed
name: University Of Minnesota Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Minnesota, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Minnesota
provider_slug: university-of-minnesota
slug: university-of-minnesota-domain-security
source_filename: university-of-minnesota-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: twin-cities.umn.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 05:47:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sites.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: integration-boomi.umn.edu\n  https: false\ndomains:\n- domain: umn.edu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-minnesota/refs/heads/main/security/university-of-minnesota-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Geospatial
- United States
- Minnesota
---
