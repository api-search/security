---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aino.world
  spf: true
hosts:
- cert_expires: Aug 27 08:43:32 2026 GMT
  host: aino.world
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aino World Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aino World Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aino World Inc.
provider_slug: aino-world-inc
slug: aino-world-inc-domain-security
source_filename: aino-world-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aino.world\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 08:43:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aino.world\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aino-world-inc/refs/heads/main/security/aino-world-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Spatial Analytics
- Geospatial
- GIS
- Mapping
- Location Intelligence
- Urban Planning
- Real Estate
- Artificial Intelligence
- Data
---
