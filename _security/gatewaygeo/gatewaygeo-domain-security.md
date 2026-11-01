---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gatewaygeomatics.com
  spf: true
hosts:
- cert_expires: Dec  5 02:04:20 2026 GMT
  host: gatewaygeomatics.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gatewaygeo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GatewayGeo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GatewayGeo
provider_slug: gatewaygeo
slug: gatewaygeo-domain-security
source_filename: gatewaygeo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gatewaygeomatics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 02:04:20 2026 GMT\n  hsts: false\ndomains:\n- domain: gatewaygeomatics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gatewaygeo/security/gatewaygeo-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Geospatial
- Consulting
- OpenSource
- FOSS4G
---
