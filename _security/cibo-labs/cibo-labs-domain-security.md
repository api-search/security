---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cibolabs.com.au
  spf: true
hosts:
- cert_expires: Dec 25 08:50:11 2026 GMT
  host: www.cibolabs.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cibo Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cibo Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cibo Labs
provider_slug: cibo-labs
slug: cibo-labs-domain-security
source_filename: cibo-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cibolabs.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 08:50:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cibolabs.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cibo-labs/security/cibo-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agriculture
- DataAnalytics
- Geospatial
- SatelliteImagery
- FarmManagement
---
