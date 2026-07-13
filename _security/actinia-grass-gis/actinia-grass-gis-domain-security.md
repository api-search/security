---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mundialis.de
  spf: true
hosts:
- cert_expires: Sep 14 12:11:18 2026 GMT
  host: actinia.mundialis.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Actinia Grass Gis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Actinia Grass GIS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Actinia Grass GIS
provider_slug: actinia-grass-gis
slug: actinia-grass-gis-domain-security
source_filename: actinia-grass-gis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: actinia.mundialis.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:11:18 2026 GMT\n  hsts: false\ndomains:\n- domain: mundialis.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actinia-grass-gis/refs/heads/main/security/actinia-grass-gis-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geocoding
- Public APIs
---
