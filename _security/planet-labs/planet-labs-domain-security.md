---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: planet.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.planet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 17:13:15 2026 GMT
  host: docs.planet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 20:29:45 2026 GMT
  host: api.planet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Planet Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Planet Labs, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Planet Labs
provider_slug: planet-labs
slug: planet-labs-domain-security
source_filename: planet-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.planet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.planet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 17:13:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.planet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 20:29:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: planet.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planet-labs/refs/heads/main/security/planet-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Earth Observation
- Satellite Imagery
- Geospatial
- PlanetScope
- SkySat
- Pelican
- Tasking
- Basemaps
- Analytics
- Subscriptions
- STAC
- GIS
---
