---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: overturemaps.org
  spf: true
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: overturemaps.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 02:56:50 2026 GMT
  host: docs.overturemaps.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 01:02:19 2026 GMT
  host: explore.overturemaps.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Overture Maps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Overture Maps Foundation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Overture Maps Foundation
provider_slug: overture-maps
slug: overture-maps-domain-security
source_filename: overture-maps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: overturemaps.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: false\n- host: docs.overturemaps.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 02:56:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: explore.overturemaps.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 01:02:19 2026 GMT\n  hsts: false\ndomains:\n- domain: overturemaps.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/overture-maps/refs/heads/main/security/overture-maps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Maps
- Geospatial
- Open Data
- GeoParquet
- Open Source
- Linux Foundation
---
