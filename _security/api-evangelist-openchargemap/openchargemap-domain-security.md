---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openchargemap.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: openchargemap.io
  spf: false
hosts:
- cert_expires: Jul 15 20:07:13 2026 GMT
  host: openchargemap.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 17:01:01 2026 GMT
  host: api.openchargemap.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openchargemap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Charge Map, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Charge Map
provider_slug: api-evangelist-openchargemap
slug: openchargemap-domain-security
source_filename: openchargemap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openchargemap.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 15 20:07:13 2026 GMT\n  hsts: false\n- host: api.openchargemap.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 17:01:01 2026 GMT\n  hsts: null\ndomains:\n- domain: openchargemap.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openchargemap.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-evangelist-openchargemap/refs/heads/main/security/openchargemap-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Electric Vehicles
- EV Charging
- Charging Stations
- Points of Interest
- Open Data
- Geospatial
- Transportation
- Clean Energy
- Crowdsourced
- Registry
---
