---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: usgif.org
  spf: true
hosts:
- cert_expires: Jan 10 21:36:59 2027 GMT
  host: www.usgif.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: U S Geospatial Intelligence Foundation Usgif Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for U.S. Geospatial Intelligence Foundation (USGIF), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: U.S. Geospatial Intelligence Foundation (USGIF)
provider_slug: u-s-geospatial-intelligence-foundation-usgif
slug: u-s-geospatial-intelligence-foundation-usgif-domain-security
source_filename: u-s-geospatial-intelligence-foundation-usgif-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usgif.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 21:36:59 2027 GMT\n  hsts: false\ndomains:\n- domain: usgif.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/u-s-geospatial-intelligence-foundation-usgif/security/u-s-geospatial-intelligence-foundation-usgif-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Geospatial
- Intelligence
- Nonprofit
- Community
---
