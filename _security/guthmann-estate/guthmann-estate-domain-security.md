---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: guthmann.estate
  spf: true
hosts:
- cert_expires: Feb  8 21:37:43 2027 GMT
  host: guthmann.estate
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Guthmann Estate GmbH Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Guthmann Estate GmbH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Guthmann Estate GmbH
provider_slug: guthmann-estate
slug: guthmann-estate-domain-security
source_filename: guthmann-estate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: guthmann.estate\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 21:37:43 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: guthmann.estate\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/guthmann-estate/security/guthmann-estate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real Estate
- Berlin
- Property
- Agency
---
