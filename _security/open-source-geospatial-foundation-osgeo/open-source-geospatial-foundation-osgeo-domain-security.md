---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: osgeo.org
  spf: true
hosts:
- cert_expires: Dec 15 15:47:00 2026 GMT
  host: www.osgeo.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Source Geospatial Foundation Osgeo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Source Geospatial Foundation (OSGeo), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Open Source Geospatial Foundation (OSGeo)
provider_slug: open-source-geospatial-foundation-osgeo
slug: open-source-geospatial-foundation-osgeo-domain-security
source_filename: open-source-geospatial-foundation-osgeo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.osgeo.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 15:47:00 2026 GMT\n  hsts: false\ndomains:\n- domain: osgeo.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/open-source-geospatial-foundation-osgeo/security/open-source-geospatial-foundation-osgeo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geospatial
- Open Source
- Foundation
- Community
- GIS
---
