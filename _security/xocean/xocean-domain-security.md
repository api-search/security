---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xocean.com
  spf: true
hosts:
- cert_expires: Nov  4 23:06:16 2026 GMT
  host: xocean.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xocean Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XOCEAN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: XOCEAN
provider_slug: xocean
slug: xocean-domain-security
source_filename: xocean-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xocean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:06:16 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: xocean.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xocean/refs/heads/main/security/xocean-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ocean Data
- Marine Survey
- Hydrography
- Uncrewed Surface Vessels
- Marine Robotics
- Offshore Wind
- Seabed Mapping
- Bathymetry
- Geospatial
- Environmental Monitoring
- Subsea Cables
- Carbon Capture and Storage
- Blue Economy
- Ireland
---
