---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mantari.com
  spf: true
hosts:
- cert_expires: Oct 10 00:17:28 2026 GMT
  host: www.mantari.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mantari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mantari, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mantari
provider_slug: mantari
slug: mantari-domain-security
source_filename: mantari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mantari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 00:17:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mantari.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mantari/refs/heads/main/security/mantari-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Weather Intelligence
- Earth Observation
- Sensors
- Artificial Intelligence
- Geospatial
- Decision Intelligence
- Defense
---
