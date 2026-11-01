---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lat-lon.de
  spf: true
hosts:
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: www.lat-lon.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lat Lon Gmbh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lat/lon GmbH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: lat/lon GmbH
provider_slug: lat-lon-gmbh
slug: lat-lon-gmbh-domain-security
source_filename: lat-lon-gmbh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lat-lon.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lat-lon.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/lat-lon-gmbh/security/lat-lon-gmbh-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- GIS
- Open-Source
- Consulting
- Geodata
---
