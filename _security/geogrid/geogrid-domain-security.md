---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: egeogrid.com
  spf: true
hosts:
- cert_expires: Sep 17 02:31:57 2026 GMT
  host: www.egeogrid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geogrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GeoGrid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GeoGrid
provider_slug: geogrid
slug: geogrid-domain-security
source_filename: geogrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.egeogrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 02:31:57 2026 GMT\n  hsts: false\ndomains:\n- domain: egeogrid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geogrid/refs/heads/main/security/geogrid-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Water Management
- Water Purification
- Smart Building
- IoT
- Water Quality Monitoring
- ESG
- Korea
---
