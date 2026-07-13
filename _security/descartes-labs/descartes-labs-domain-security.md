---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: descarteslabs.com
  spf: false
hosts:
- cert_expires: Dec 31 15:31:47 2026 GMT
  host: www.descarteslabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Descartes Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Descartes Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Descartes Labs
provider_slug: descartes-labs
slug: descartes-labs-domain-security
source_filename: descartes-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.descarteslabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 15:31:47 2026 GMT\n  hsts: false\ndomains:\n- domain: descarteslabs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/descartes-labs/refs/heads/main/security/descartes-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geospatial
- Geospatial Intelligence
- Earth Observation
- Satellite Imagery
- Remote Sensing
- Raster
- Vector
- GIS
- Machine Learning
- Geospatial Analytics
- Agriculture
- Mining
- Energy
- Defense
- Climate
- Acquired
- EarthOne
- EarthDaily
- Discontinued
---
