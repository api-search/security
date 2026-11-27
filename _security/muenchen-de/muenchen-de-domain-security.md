---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: muenchen.de
  spf: true
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: opendata.muenchen.de
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Landeshauptstadt München Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Landeshauptstadt München, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Landeshauptstadt München
provider_slug: muenchen-de
slug: muenchen-de-domain-security
source_filename: muenchen-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.muenchen.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: muenchen.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/muenchen-de/security/muenchen-de-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Open Data
- Municipal
- CKAN
- Geospatial
- OGC
- Germany
- Munich
---
